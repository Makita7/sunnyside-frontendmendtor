<script>
    import { ref } from 'vue';
    import Emily from '../assets/image-emily.jpg'
    import Thomas from '../assets/image-thomas.jpg'
    import Jennie from '../assets/image-jennie.jpg'

    export default{
        name: 'clients',
        data(){
            return{
                Info: ref([
                    {
                        id:1,
                        photo: Emily,
                        comment: 'We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.',
                        client: 'emily r.',
                        position: 'marketing director',
                    },
                    {
                        id:2,
                        photo: Thomas,
                        comment: `Sunnyside's enthusiasm coupled with their keen interest in our brand's success made it a satisfying and enjoyable experience`,
                        client: 'thomas s.',
                        position: 'chief operating officer',
                    },
                    {
                        id:3,
                        photo: Jennie,
                        comment: 'Incredible end result! Our sales increased over 400% when we worked with Sunnyside. Highly recommended!',
                        client: 'jennie f.',
                        position: 'business owner',
                    },
                ])}
            }
    }
</script>

<template>
    <div class="client">
        <h4>Client Testimonials</h4>
        <div class="flex evenly">
            <div class="card" v-for="(item in Info">
                <img :alt="item.client" :src="item.photo" />
                <p class="comment">{{item.comment}}</p>
                <h5>{{item.client}}</h5>
                <p class="position">{{item.position}}</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .client{
        min-height: 28rem;
        padding: 5rem;
    }
    .client h4 {
        text-transform: uppercase;
        text-align: center;
        font-size: 1.2rem;
        color: var(--GrayishBlue);
        padding-top: 2rem;
    }
    .client .card{
        width: 23rem;
        margin: 3rem 0rem;
        display: block;
        text-align: center;
    }
    .client .card img {
        border-radius: 50px;
        height: 4rem;
    }
    .client .card .comment {
        font-weight: 600;
        padding: 2rem 0;
        color: var(--DarkGrayishBlue);
    }
    .client .card .position {
        color: var(--GrayishBlue);
        font-size: 1rem;
        font-weight: 600;
        padding-top: 0.2rem;
    }
    .client .card h5 {
        color: var(--DarkBlue);
        font-size: 1.5rem;
        text-transform: capitalize;
    }
</style>