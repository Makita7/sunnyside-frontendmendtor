
<template>
    <section class="sectTwo">
        <div class="flex">
            <div class="containerTwo">
                    <img class="back" alt='graphic design' src='../assets/desktop/image-graphic-design.jpg' />
                    <h3 class="overTitle">Graphic Design</h3>
                    <p class="overP">
                        Great design makes you memorable. We deliver artwork that underscores your brand message and captures potential client's attention.
                    </p>
            </div>

            <div class="container">
                <img alt='photography' src='../assets/desktop/image-photography.jpg' />
                <h3 class="overTitle">Photography</h3>
                <p class="overP">
                    Increase your credibility by getting the most stunning, high-quality photos that improve your business image.
                </p>
            </div>
        </div>
    </section>
</template>

<style>
    .sectTwo{
        margin-top: -1rem;
        color: var(--DarkDesaturatedCyan);
    }
    .containerTwo{
        width: 50%;
    }
    .sectTwo img{
        width: 100%;
    }
    .back{
        position: relative;
        z-index: 0;
    }
    .overTitle {
        position: absolute;
        z-index: +5;
        margin-top: -12rem;
        width: 50%;
        text-align: center;
    }
    .overP {
        position: absolute;
        z-index: +5;
        margin-top: -8rem;
        width: 27%;
        text-align: center;
        margin-left: 11.5%;
        font-weight: 600;
    }
</style>
