<script>
import { ref } from 'vue';
import IconF from '../assets/icon-facebook.svg';
import IconI from '../assets/icon-instagram.svg';
import IconP from '../assets/icon-pinterest.svg';
import IconT from '../assets/icon-twitter.svg';


    export default{
        data(){
            return{
                social: ref([
                    {
                        id: 1,
                        link: 'https://www.facebook.com',
                        icon: "fa-brands fa-square-facebook",
                        alt: 'facebook',
                    },
                    {
                        id: 2,
                        link: 'https://www.instagram.com',
                        icon: 'fa-brands fa-instagram',
                        alt: 'instagram',
                    },
                    {
                        id: 3,
                        link: 'https://www.twitter.com',
                        icon: 'fa-brands fa-twitter',
                        alt: 'twitter',
                    },
                    {
                        id: 4,
                        link: 'https://www.pinterest.com',
                        icon: 'fa-brands fa-pinterest',
                        alt: 'pinterest',
                    },
                ])
            }
        }
    }
</script>

<template>
    <footer>
        <img class="logo" src="../assets/logo.svg" />
        <ul class="flex">
            <li>About</li>
            <li>Services</li>
            <li>Projects</li>
        </ul>
        <div class="inlineFlex" v-for="items in social">
            <a :href="items.link" :id="items.id">
                <font-awesome-icon :icon="items.icon" size="lg" />
            </a>
        </div>
    </footer>
</template>

<style scoped>
    footer{
        min-height: 22rem;
        background-color: #90d4c5;
        color: var(--DarkModerateCyan);
        text-align: center;
    }
    .inlineFlex{
        display: inline-flex;
        padding: 0 1rem;
    }
    footer li {
        list-style: none;
        padding: 0 2rem;
        font-weight: 600;
        font-family: 'Barlow', sans-serif;
        font-weight: 600;
    }
    .svg-inline--fa.fa-lg {
        color: var(--DarkModerateCyan);
    }
    .svg-inline--fa.fa-lg:hover{
        color: white;
        transition: 0.5s;
    }
    footer ul {
        margin-left: 36%;
        margin-right: auto;
        padding-top: 2.5rem;
        padding-bottom: 5rem;
    }
    footer .logo {
        fill: var(--DarkModerateCyan);
        margin-top: 4rem;
        height: 2.5rem;
    }
    footer .logo{
        fill: var(--DarkModerateCyan);
    }

    a:hover{
        color: white;
    }

    footer li:hover{
        color: white;
        transition: 0.5s;
    }

    @media only screen and  (min-width:1900px){
        footer ul {
            margin-left: 39%;
        }
    }

    @media only screen and (max-width: 1023px) {
        footer ul {
            margin-left: 24%;
        }
    }
    @media only screen and (max-width: 767px) {
        footer ul {
        margin-left: 5%;
        }
        footer li{
            padding: 0 1rem;
        }
    }
</style>