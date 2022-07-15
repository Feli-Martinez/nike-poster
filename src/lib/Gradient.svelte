<script>
    export let firstColor, secondColor, thirdColor;

    export let verticalPosition = "top";
    export let horizontalPosition = "left";

    let opposites = {
        "top": "bottom",
        "bottom": "top",
        "left": "right",
        "right": "left"
    };
</script>

<div class="Gradient" style="
    {horizontalPosition}: 0;
    {verticalPosition}: 0;
    background: linear-gradient(to {opposites[verticalPosition]} {opposites[horizontalPosition]}, {firstColor} 35%, {secondColor}, {thirdColor} 73%);
"></div>

<style>
    .Gradient{
        position: absolute;
        width: 55%;
        height: 51%;
        border-radius: 5%;
        filter: blur(71px);
    }
</style>