<script>
    import {page} from '$app/stores';
    import logo from '$lib/images/svelte-logo.svg';
    import github from '$lib/images/github.svg';
</script>

<header>
    <nav>
        <ul class="navbar-menu">
            <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
                <a href="/">Home</a>
            </li>
            <li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
                <a href="/about">About</a>
            </li>
            <li aria-current={$page.url.pathname === '/bulma' ? 'page' : undefined}>
                <a href="/bulma">Bulma</a>
            </li>
            <li aria-current={$page.url.pathname.startsWith('/spectre') ? 'page' : undefined}>
                <a href="/spectre">Spectre</a>
            </li>
            <li aria-current={$page.url.pathname.startsWith('/picocss') ? 'page' : undefined}>
                <a href="/picocss">Picocss</a>
            </li>
            <li aria-current={$page.url.pathname.startsWith('/skeleton') ? 'page' : undefined}>
                <a href="/skeleton">Skeleton</a>
            </li>
        </ul>
    </nav>
</header>

<style>
    /**
    Estilos
    */
</style>
