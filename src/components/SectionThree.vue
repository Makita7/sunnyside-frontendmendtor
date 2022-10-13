
<template>
    <div class="flex">
        <img alt="milk botles" src="../assets/desktop/image-gallery-milkbottles.jpg" class="dividedFour"/>
        <img alt="milk botles" src="../assets/desktop/image-gallery-orange.jpg" class="dividedFour"/>
        <img alt="milk botles" src="../assets/desktop/image-gallery-cone.jpg" class="dividedFour"/>
        <img alt="milk botles" src="../assets/desktop/image-gallery-sugarcubes.jpg" class="dividedFour"/>
    </div>
</template>

<style scoped>
    .dividedFour{
        width: 25%;
        height: auto;
    }
    @media only screen and (max-width: 767px) {
        .dividedFour{
            width: 50%;
        }
        footer li {
            padding: 0 1rem;
        }
        footer ul{
            margin-left: 5%;
        }
    }
</style>