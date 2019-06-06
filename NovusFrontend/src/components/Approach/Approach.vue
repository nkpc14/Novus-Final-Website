<template>
    <div>
        <div class="divider">
            <h3>Approach</h3>
            <hr>
        </div>
        <div class="approach">

            <div class="approach__content">
                <img src="../../assets/images/Ellipse_oragange.png" alt="">
                <h1> We are driven by passion and believe in innovation.</h1>
                <p> We are currently having our studio in Punjab, India. Our experienced team is capable enough
                    to take up clients from all around the globe. So if your from foreign country, you’re
                    most welcome.
                </p>
            </div>
            <div class="approach__circle">
                <img class="approach__circle-1" src="../../assets/images/Ellipse_empty.png" alt="">
                <img class="approach__circle-2" src="../../assets/images/Ellipse_empty.png" alt="">
                <img class="approach__circle-3" src="../../assets/images/Ellipse_empty.png" alt="">
            </div>

            <div class="approach__map">
                <img  src="../../assets/images/world.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Approach"
    }
</script>

<style scoped lang="scss">
    .divider{
        margin: 15rem 6rem 0 6rem;
        font-family: Poppins,sans-serif;

    }
    hr{
        height: 0.01rem;
        margin-bottom: 10rem;
        color: white;
        background-color: white;
    }

    .approach{
        height: 100vh;
        padding: 6rem;
        font-family: Poppins,sans-serif;
        display: grid;
        grid-template-columns: auto auto auto auto auto;
        grid-template-rows: auto 20rem auto auto;
        &__content{
            grid-column: 1/3;
            grid-row:1/2;
            padding: 4rem;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            /*background-color: red;*/
            height: 30rem;
            position: relative;
            & img{
                position: absolute;
                top: 0;
                left: 0;
            }
            & h1{
                font-size: 5rem;
                z-index: 2;
            }

            & p{
                font-size: 1.8rem;
                max-width: 62rem;
                z-index: 2;
            }
        }

        &__circle{
            grid-column: 3/6;
            grid-row: 1/2;

            &-1{
                transform: translate(8rem,0rem);
            }
            &-2{

            }
            &-3{
                transform: translate(-46rem,18rem);
            }
        }

        &__map{
            grid-column: 2/5;
            grid-row: 4/5;
        }
    }
</style>