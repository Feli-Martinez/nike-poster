<script>
    import CardHeader from "$lib/CardHeader.svelte";
    import CardBody from "$lib/CardBody.svelte";
    import CardFooter from "$lib/CardFooter.svelte";
</script>

<div class="Card">
    <CardHeader />
    <CardBody />
    <CardFooter />
</div>

<style>
    .Card{
        position: absolute;
        width: 950px;
        height: 605px;
        left: calc(50% - 450px);
        background: linear-gradient(to right, rgb(255, 255, 255, 0.28) 0%, rgb(255, 255, 255, 0) 100%);
        backdrop-filter: blur(800px);
        border-radius: 40px;
        border: 2px solid #fff;
    }
</style>