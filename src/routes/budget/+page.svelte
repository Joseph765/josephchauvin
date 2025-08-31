<script>
    import Nav from "../Nav.svelte";
    import { Divider, Flex } from "$lib/components";

    let checking = '';
    let savings = '';
    let monthlySpending = '';
    let error = '';
    let submitted = false;

    let total = 0;
    let projections = [];
    let monthsUntilZero = 0;
    let finalDate = '';

    function handleSubmit() {
        // Reset error and projections
        error = '';
        projections = [];
        monthsUntilZero = 0;
        finalDate = '';
        submitted = true;

        // Validate inputs
        if (!checking || isNaN(checking) || parseFloat(checking) < 0) {
            error = 'Please enter a valid non-negative number for checking account';
            submitted = false;
            return;
        }
        if (!savings || isNaN(savings) || parseFloat(savings) < 0) {
            error = 'Please enter a valid non-negative number for savings account';
            submitted = false;
            return;
        }
        if (!monthlySpending || isNaN(monthlySpending) || parseFloat(monthlySpending) <= 0) {
            error = 'Please enter a valid positive number for monthly spending';
            submitted = false;
            return;
        }

        // Calculate total and projections
        total = parseFloat(checking) + parseFloat(savings);
        const today = new Date();
        let balance = total;
        let i = 0;

        // Generate projections for 30-day intervals until balance is close to zero
        while (balance > 0 && i < 1000) {
            const futureDate = new Date(today);
            futureDate.setDate(today.getDate() + i * 30);
            const year = futureDate.getFullYear().toString().slice(-2);
            const formattedDate = `${futureDate.toLocaleString('en-US', { month: 'short', day: 'numeric' })}, '${year}`;
            projections.push({ date: formattedDate, balance });
            balance -= parseFloat(monthlySpending);
            i++;
        }

        // Calculate exact date when balance reaches zero or goes negative
        if (i < 1000) {
            const lastBalance = projections.length > 0 ? projections[projections.length - 1].balance : total;
            const remainingDays = (lastBalance / parseFloat(monthlySpending)) * 30; // Proportion of month remaining
            const finalProjectionDate = new Date(today);
            finalProjectionDate.setDate(today.getDate() + ((i - 1) * 30 + Math.floor(remainingDays)));
            const year = finalProjectionDate.getFullYear().toString().slice(-2);
            const formattedDate = `${finalProjectionDate.toLocaleString('en-US', { month: 'short', day: 'numeric' })}, '${year}`;
            projections.push({ date: formattedDate, balance: 0 }); // Add zero balance entry
        }

        // Calculate months until zero and final date for stat card
        monthsUntilZero = i - 1 + (projections.length > 1 ? (projections[projections.length - 1].balance === 0 ? 1 : 0) : 0);
        if (projections.length > 1) {
            const finalProjectionDate = new Date(today);
            finalProjectionDate.setDate(today.getDate() + ((i - 1) * 30 + Math.floor(remainingDays)));
            finalDate = finalProjectionDate.toLocaleString('en-US', { month: 'long', day: 'numeric', year: 'numeric' });
        } else {
            finalDate = today.toLocaleString('en-US', { month: 'long', day: 'numeric', year: 'numeric' });
        }
    }
</script>

<div class="layout">
    <Nav />
    <div class="section">
        <div>
            <Flex direction="column">
                <Flex gap="s" direction="column">
                    <label for="savings">Savings Account Balance</label>
                    <input type="number" id="savings" placeholder="55000.00" bind:value={savings} min="0" step="0.01" />
                </Flex>
                <Flex gap="s" direction="column">
                    <label for="checking">Checking Account Balance</label>
                    <input type="number" id="checking" placeholder="10000.00"  bind:value={checking} min="0" step="0.01" />
                </Flex>
                <Flex gap="s" direction="column">
                    <label for="monthlySpending">Monthly Budget</label>
                    <input type="number" id="monthlySpending" placeholder="3000.00" bind:value={monthlySpending} min="0.01" step="0.01" />
                </Flex>
                <Flex gap="s" direction="column">
                    <button on:click={handleSubmit}>Submit</button>
                    {#if error}
                        <p style="color: red;">{error}</p>
                    {/if}
                </Flex>
            </Flex>
        </div>
    </div>
    {#if submitted && projections.length > 0}
        <Divider />
        <div class="section">
            <Flex direction="column">
                <h2>Financial Projection</h2>
                <div class="stat-card">
                    <p class="stat-label">Months until $0 balance</p>
                    <p class="stat">{monthsUntilZero}</p>
                </div>
                <div class="stat-card">
                    <p class="stat-label">Date of $0 balance</p>
                    <p class="stat">{projections[projections.length - 1].date}</p>
                </div>
                <table>
                    <thead>
                        <tr>
                            <th>Date</th>
                            <th>Balance</th>
                        </tr>
                    </thead>
                    <tbody>
                        {#each projections as proj, i}
                            <tr>
                                <td>{proj.date}</td>
                                <td class={i === projections.length - 1 ? "is-danger" : ""}>${proj.balance.toLocaleString('en-US', { minimumFractionDigits: 2, maximumFractionDigits: 2 })}</td>
                            </tr>
                        {/each}
                    </tbody>
                </table>
            </Flex>
        </div>
    {/if}
</div>

<style>
    .layout {
        color: var(--color-text);
        overflow: hidden;
        padding-block-start: var(--header-height);
        font-family: var(--font-family);
    }

    .section {
        padding: 1rem 1rem;
    }

    button {
        border: none;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
        height: 3rem;
        width: 100%;
        color: var(--color-text);
        font-family: var(--font-family);
        font-size: 1rem;
        padding: 0.5rem 1rem;
        border-radius: 2px;
        background: var(--color-accent);
    }

    input {
        height: 2rem;
        font-size: 1rem;
        border: 1px solid var(--color-border);
        border-radius: 2px;
        background: var(--color-surface);
    }

    input::placeholder {
        color: var(--gray-6); /* Sets the placeholder text color to red using a hex code */
    }

    .stat-card {
        display: flex;
        flex-direction: column;
        gap: var(--space-s);
        border: 1px solid var(--color-border);
        border-radius: 2px;
        background: var(--color-surface);
        padding: 1rem;
    }

    .stat-label {
        font-size: 1rem;
        color: var(--color-text-weak);
    }

    .stat {
        font-size: 1.5rem;
        color: var(--color-text);
    }

    table {
        border-collapse: collapse;
        width: 100%;
        color: var(--color-text);
    }

    .is-danger {
        color: var(--color-text-danger);
    }

    th, td {
        border: 1px solid var(--color-border);
        padding: 8px;
        text-align: left;
        background: var(--color-surface);
    }

    th {
        background-color: var(--color-surface-raised);
    }
</style>