
<script>
    import { Divider } from "$lib/components";
</script>

<Divider />
<footer>
    <a aria-label="YouTube" target="_blank" href="https://www.youtube.com/@josephchauvin1973">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-youtube-icon lucide-youtube"><path d="M2.5 17a24.12 24.12 0 0 1 0-10 2 2 0 0 1 1.4-1.4 49.56 49.56 0 0 1 16.2 0A2 2 0 0 1 21.5 7a24.12 24.12 0 0 1 0 10 2 2 0 0 1-1.4 1.4 49.55 49.55 0 0 1-16.2 0A2 2 0 0 1 2.5 17"/><path d="m10 15 5-3-5-3z"/></svg>
    </a>
    <a aria-label="Spotify" target="_blank" href="https://open.spotify.com/artist/0RvAlcc5b1AgsrLJyQDCkP?si=Ig8qY691R9CdzbNEf-GMPQ">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-music-icon lucide-music"><path d="M9 18V5l12-2v13"/><circle cx="6" cy="18" r="3"/><circle cx="18" cy="16" r="3"/></svg>
    </a>
    <a aria-label="Instagram" target="_blank" href="https://www.instagram.com/_joseph_chauvin/">
        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-instagram-icon lucide-instagram"><rect width="20" height="20" x="2" y="2" rx="5" ry="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" x2="17.51" y1="6.5" y2="6.5"/></svg>
    </a>
</footer>


<style>
    footer {
        padding-block: 4rem;
        background-color: var(--color-background);
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 1rem;
    }

    a {
        color: var(--color-text);
        text-decoration: none;
    }

    a:hover {
        color: var(--indigo-12);
    }
</style>