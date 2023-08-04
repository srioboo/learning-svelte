<script>
    import {page} from '$app/stores';
    import logo from '$lib/images/svelte-logo.svg';
    import github from '$lib/images/github.svg';
</script>

<header>
    <nav>
        <ul class="corner">
            <li><a href="https://kit.svelte.dev">
                Svelte Kit
            </a></li>
        </ul>
        <ul class="navbar-menu">
            <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
                <a href="/">Home</a>
            </li>
            <li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
                <a href="/about">About</a>
            </li>
            <li aria-current={$page.url.pathname.startsWith('/sverdle') ? 'page' : undefined}>
                <a href="/sverdle">Sverdle</a>
            </li>
        </ul>
        <ul class="corner">
            <li><a href="https://github.com/sveltejs/kit">
                GitHub Svelkit
            </a></li>
        </ul>
    </nav>
</header>

<style>
    /**
    Estilos
    */
</style>
