
<template>
    <section class="sectOne">
        <div class="flex">
            <div class="container text">
                <h3>Transform your brand</h3>
                <p>We are a full-service creative agency specializing in helping brands grow fast. Engage your clients through compelling visuals that do most of the marketing for you.</p>
                <a href="">
                    Learn more
                    <div class="yellow"></div>
                </a>
            </div>
            <div class="container">
                <img alt='transform' src='../assets/desktop/image-transform.jpg' />
            </div>
        </div>
        <div class="flex">
            <div class="container">
                <img alt='stand out' src='../assets/desktop/image-stand-out.jpg' />
            </div>
            <div class="container text">
                <h3>Stand out to the right audience</h3>
                <p>Using a collaborative formula of designers, researchers, photographers and copywriters, we'll build and extend your brand in digital places.</p>
                <div>
                    <a href="">
                        Learn more
                        <div class="pink"></div>
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>

<style>
    .sectOne{
        margin-top: -1rem;
    }
    .sectOne p{
        color: var(--DarkGrayishBlue);
        font-weight: 600;
        padding: 2rem 0;
    }
    .sectOne img{
        width: 100%;
    }
    .container{
        width: 50%;
        box-sizing: border-box;
    }
    .sectOne .text {
    padding: 8%;
    margin-top: auto;
    margin-bottom: auto;
    }
    .sectOne h3{
        font-size: 3rem;
        color: var(--VeryDarkDesaturatedBlue);
    }
    .sectOne a{
        color: var(--VeryDarkDesaturatedBlue);
        text-decoration: none;
    }
    .yellow {
        background-color: var(--Yellow) !important;
        height: 1rem;
        width: 25%;
        border-radius: 6px;
        margin-top: -0.6rem;
        margin-left: -0.3rem;
    }
    .pink {
        background-color: var(--SoftRed) !important;
        height: 1rem;
        width: 25%;
        border-radius: 6px;
        margin-top: -0.6rem;
        margin-left: -0.3rem;
    }
</style>