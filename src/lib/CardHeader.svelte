<script>
    import HeaderList from "$lib/HeaderList.svelte";
    import Button from "$lib/Button.svelte";
</script>

<div class="Card__header">
    <img src="Logo.svg" alt="nike logo" class="header__logo">
    <HeaderList />
    <div class="search_n_shop">
        <Button icon='Search.svg' text='Search' glow={false} />
        <div class="separator"></div>
        <Button text='Shop Now' bgColor="#FF64A5" />
    </div>
</div>

<style>
    .Card__header{
        position: relative;
        display: flex;
        margin: 15px;
        margin-top: 27px;
        margin-left: -15px;
    }

    .header__logo{
        width: 200px;
        height: 34px;
        margin-top: 3.5px;
    }

    .search_n_shop{
        position: absolute;
        display: flex;
        right: 25px;
    }

    .separator{
        margin-left: 30px;
    }
</style>