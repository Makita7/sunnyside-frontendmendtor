<script>
    import Navbar from './Navbar.vue';
    export default{
        components: {
            Navbar: Navbar,
        }
    }
</script>

<template>
    <header>
        <Navbar/>
        <img
        alt="banner"
        src="../assets/desktop/imageHeader.jpg"
        />
        <div class="over">
        <h1 class="over">We are creatives</h1>
        <img class="arrow" alt="arrow" src="../assets/icon-arrow-down.svg" />
        </div>
    </header>
</template>

<style>
    header{
        position: relative !important;
    }
    header img{
        width: 100%;
    }
    .over {
        position: absolute;
        text-align: center;
        color: white;
        z-index: +2;
        top: 20%;
        width: 100%;
        font-size: 5rem !important;
        margin-left: auto;
        margin-right: auto;
    }
    .over h1{
        width: 100%;
    }
    .arrow {
        max-width: 2rem;
        padding-top: 14rem;
    }
</style>