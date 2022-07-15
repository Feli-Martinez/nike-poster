<script>
    import Gradient from "$lib/Gradient.svelte";

    export let sizes;
</script>

<div class="Background" style="width: {sizes.width}; height: {sizes.height};">
    <Gradient firstColor="#BD00FF" secondColor="#DC0086" thirdColor="#2400FF" />
    <Gradient horizontalPosition="right" verticalPosition="bottom" firstColor="#BD00FF" secondColor="#DC0086" thirdColor="#2400FF" />
</div>

<style>
    .Background{
        position: relative;
        margin: 0 auto;
    }
</style>