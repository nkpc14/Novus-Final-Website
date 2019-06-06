<template>
    <div class="mainSection">
        <div>
            <Header></Header>
            <div class="mainSection__top">
                <div class="mainSection__top--content">

                    <h1>
                        <span class="mainSection__top--content-novus">Novus</span>
                        is a digital studio
                        that develop websites and
                        Mobile applications.

                    </h1>

                </div>
                <div class="mainSection__top--arts">
                    <img class="mainSection__top--arts-semi_cir_empty" src="../../assets/images/semi_cir_empty.png" alt="">
                    <img class="mainSection__top--arts-semi_cir_fill" src="../../assets/images/semi_cir_fill.png" alt="">
                    <img class="mainSection__top--arts-rectangle" src="../../assets/images/rectangle.png" alt="">
                    <img class="mainSection__top--arts-Ellipse" src="../../assets/images/Ellipse.png" alt="">
                    <img class="mainSection__top--arts-dots" src="../../assets/images/dots.png" alt="">
                </div>
            </div>
        </div>



        <div class="mainSection__bottom">

            <div class="mainSection__bottom--scroll">
                <p>
                    NOVUS is a student organisation since 2017 led by aspiring minds. We are pushing its limits
                    with the help of each and every determined mind that makes us, the NOVUS.
                </p>
                <div class="mainSection__bottom--scroll-in">
                    <p>Scroll to see more</p>
                    <img src="../../assets/images/Arrow.png" alt="">
                </div>
            </div>

            <div class="mainSection__bottom--photo">
                <p>
                    Innovation drives us and we are hunting for it; hunting hunting for people who stand
                    out in crowd, like you.
                </p>

                <a href="">View Photos / videos</a>

            </div>

            <div class="mainSection__bottom--video">

                <img src="../../assets/images/video.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
    import Header from './Header'
    export default {
        name: "MainSection",
        components:{
            Header
        }
    }
</script>

<style scoped lang="scss">

    .mainSection{
        /*background-color: green;*/
        height: 100vh;
        display: flex;
        flex-direction: column;

        &__top{
            display: flex;
            justify-content: space-between;
            &--content{
                padding: 6rem;
                & h1{
                    font-family: Poppins,sans-serif;
                }
                &-novus{
                    border-top:solid #FF4E00 0.2rem;
                }
            }

            &--arts{
                position: relative;
                min-width: 40%;
                /*background-color: red;*/
                & img{
                    position: absolute;
                    top: 40%;
                }

                &-semi_cir_empty{
                    margin-top: -6rem;
                    margin-left: -4rem;;
                }
                &-semi_cir_fill{
                    margin-top: 18rem;
                    margin-left: -7rem;;
                }
                &-rectangle{
                    margin-top: 10rem;
                    margin-left: 7rem;;
                }
                &-Ellipse{
                    margin-top: -2rem;
                    margin-right: -3rem;;
                }
                &-dots{
                    margin-top: 4rem;
                    margin-left: 10rem;;
                }

            }
        }


    &__bottom{
            display: flex;
            background-color: red;
            padding:8rem 4rem 0rem 4rem;
            font-size: 1.2rem;
            font-family: Poppins,sans-serif;
            &--scroll{
                display: flex;
                flex-direction: column;
                justify-content: space-between;
                padding: 2rem;
                max-width: 30vw;
                & p{
                    margin-top: 3rem;
                }

                &-in{
                    display: flex;
                }
            }

            &--photo{
                display: flex;
                flex-direction: column;
                justify-content: space-between;
                padding: 2rem;
                max-width: 25vw;
                & p{
                    margin-top: 3rem;
                }

                & a{
                    color: #fff;
                    border: solid #FF4E00 0.01rem;
                    width: 15rem;
                    padding: 0.6rem;
                    text-align: center;
                }
            }

            &--video{
                height: 30rem;
                & img{
                    height: 25rem;
                    transform: translate(0rem,6rem);
                }
            }
        }
    }

</style>
