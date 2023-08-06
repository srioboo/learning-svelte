<script>
    import './styles-bulma.scss';
</script>

<svelte:head>
    <title>Bulma test page</title>
    <meta name="description" content="Bulma test page" />
</svelte:head>


<section class="hero is-warning">
    <div class="hero-body">
        <p class="title">
            Ejemplos bulma
        </p>
        <p class="subtitle">
            Algunos ejemplos de estilos con bulma
        </p>
    </div>
</section>

<div class="container">
    <div class="columns">
        <div class="column is-primary"><p class="bd-notification is-primary">col-1</p></div>
        <div class="column"><p class="bd-notification is-primary">col-2</p></div>
        <div class="column"><p class="bd-notification is-primary">col-3</p></div>
        <div class="column"><p class="bd-notification is-primary">col-4</p></div>
    </div>
</div>

<button class="button is-primary">
    Button
</button>
