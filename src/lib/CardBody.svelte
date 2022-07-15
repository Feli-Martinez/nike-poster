<script>
    export let text = ["NI", "KE"];

    import Details from "$lib/Details.svelte";
</script>

<div class="Card__body">
    <img src="Logo.svg" alt="logo" class="body__back_logo">
    <h2 class="body__text body__text_left">{text[0]}</h2>
    <img src="Shoe.png" alt="niek" class="body__img">
    <h2 class="body__text body__text_right">{text[1]}</h2>
    <Details title="Ultra mechanics" description="When a player steps in, a custom motor and gear train senses the tension needed by the foot" />
</div>

<style>
    .Card__body{
        position: relative;
        display: flex;
        width: 90%;
        height: 60%;
        margin: 0 auto;
        margin-top: 20px;

        /*border-radius: 120px;
        border-left: 2px solid #fff;
        border-right: 2px solid #fff;*/
    }

    .body__back_logo{
        position: absolute;
        top: 28%;
        left: calc(50% - 267px);
        width: 80%;
        opacity: 0.2;
    }

    .body__img{
        position: absolute;
        width: 550px;
        height: 550px;
        top: -50px;
        left: calc(50% - 275px);
        z-index: 3;
    }

    .body__text{
        position: absolute;
        top: 34%;
        font-size: 20rem;
        color: #fff;
    }

    .body__text_left{
        left: 183px;
        z-index: 2;
    }

    .body__text_right{
        right: 128.5px;
        -webkit-text-stroke: 8px #fff;
        letter-spacing: -18px;
        color: transparent;
        z-index: 4;
    }
</style>