<svelte:head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap" rel="stylesheet">
</svelte:head>

<script>
    import Background from '$lib/Background.svelte';
    import Card from '$lib/Card.svelte';

    let sizes = {
        width: '95%',
        height: '350px'
    }
</script>

<main>
    <Background {sizes} />
    <Card />
</main>

<style>
    :global(*){
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        font-size: 62.5%;
        font-family: Helvetica;
    }

    main{
        display: flex;
        width: 100vw;
        height: 100vh;
        flex-direction: column;
        justify-content: center;
        background-color: rgba(0, 0, 0, 0.95);
    }
</style>