<script>
    export let text, icon;
    export let glow = true;
    export let bgColor = 'transparent';

    let glowStyle = glow ? `box-shadow: 0 0 17px ${bgColor};` : ``;
</script>

<button class="Button" style="{glowStyle} background-color: {bgColor};">
    {#if icon}
        <img src="{icon}" alt="{text} icon" class="Button__icon">
    {/if}
    <h2 class="Button__text">{text}</h2>
</button>

<style>
    .Button{
        display: flex;
        width: auto;
        padding: 10px;
        border: none;
        border-radius: 7px;
    }

    .Button__icon{
        width: 20px;
        margin-right: 10px;
        align-self: baseline;
    }

    .Button__text{
        font-weight: 500;
        font-size: 2rem;
        color: #fff;
    }
</style>