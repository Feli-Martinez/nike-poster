<script>
    export let title, description;
</script>

<div class="Details">
    <h3 class="body__details_title">{title}</h3>
    <p class="body__details_desc">{description}</p>
</div>

<style>
    .Details{
        position: absolute;
        bottom: -17px;
        right: 0;
    }

    .body__details_title{
        font-size: 2rem;
        text-align: center;
    }

    .body__details_desc{
        font-size: 1.4rem;
    }
</style>