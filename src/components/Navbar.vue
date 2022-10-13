<script>
    export default{
        name: 'bugernav',
        props: {
            active: {
                type: Boolean,
                required: true,
                default: false,
            }
        },
        // methods: {
        //     toggle() {
        //         this.active = !this.active
        //         this.$emit( active, 'toggle-menu' )
        //     }
        // }
    }
</script>

<template>
    <div class="flex navbar">
        <img class="logoH" src=".././assets/logo.svg" alt='logo'/>
        <div class="links deskShow">
            <ul class="flex">
                <li class="links padFix">About</li>
                <li class="links padFix">Services</li>
                <li class="links padFix">Projects</li>
                <li class="links contact">Contact</li>
            </ul>
        </div>
        <div class="cellShow" @click.prevent="active = !active">
            <img class="hMenu" alt="burger menu" src="../assets/icon-hamburger.svg" />
        </div>
        <div class="cellShow burgerNavOpen" v-if="active">
            <ul class="">
                <li class="links padFix">About</li>
                <li class="links padFix">Services</li>
                <li class="links padFix">Projects</li>
                <li class="links padFix">Contact</li>
            </ul>
        </div>
    </div>
</template>

<style scoped>
    .navbar{
        position: absolute;
        z-index: +2;
        margin: 2rem;
        width: 100%;
    }
    .links {
        list-style: none;
        color: white;
        font-size: 1.2rem;
        margin-left: auto;
        padding: 0 1rem;
        margin-right: 1.5rem !important;
    }
    img.logoH {
        width: 12rem;
    }
    .contact {
        background-color: rgb(255, 255, 255);
        color: var(--DarkBlue);
        font-family: 'Fraunces', serif;
        font-size: 0.8rem;
        padding: 0.8rem 1.5rem;
        border-radius: 10pc;
        text-transform: uppercase;
    }
    .padFix{
        padding-top: 0.5rem;
    }
    @media only screen and (max-width: 767px) {
        img.logoH {
        width: 7rem;
        height: 1.8rem;
        }
        .hMenu{
            margin-left: 810%;
        }
        .burgerNavOpen {
            background-color: white;
            height: 20rem;
            width: 19.5rem;
            padding: 1rem;
            margin-left: -9rem;
            z-index: +10;
            position: sticky;
            margin-top: 3rem;
        }
        .burgerNavOpen li{
            color: black;
            z-index: +15;
            padding-top: 2.5rem;
            text-align: center;
            font-family: 'Barlow', sans-serif;
            font-size: 1.1rem;
            font-weight: 600;
            color: var(--DarkGrayishBlue);
        }
        .burgerNavOpen ul{
            padding-left: 0% !important;
        }
    }
</style>