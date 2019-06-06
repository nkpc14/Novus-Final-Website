<template>
   <div>
       <div           data-aos="fade-in"
                      data-aos-offset="200"
                      data-aos-delay="50"
                      data-aos-duration="400"
                      data-aos-easing="ease-in-out"
                      data-aos-mirror="true"
                      data-aos-once="false" class="divider">
           <h3>Contact Us</h3>
           <hr>
       </div>
       <div      class="contact">
           <h2        data-aos="fade-up"
                      data-aos-offset="200"
                      data-aos-delay="50"
                      data-aos-duration="400"
                      data-aos-easing="ease-in-out"
                      data-aos-mirror="true"
                      data-aos-once="false">
               So what do you say, are we the team that
               you’re looking for? <span>Contact us</span> and we
               ensure satisfaction.
           </h2>
           <div data-aos="fade-in"
                      data-aos-offset="200"
                      data-aos-delay="50"
                      data-aos-duration="400"
                      data-aos-easing="ease-in-out"
                      data-aos-mirror="true"
                      data-aos-once="false" class="contact__details">
               <div class="contact__details--about">
                   <div>
                       <h3>About Us</h3>
                       <p>
                           NOVUS is a student organisation since 2017 led
                           by aspiring minds. We are pushing its limits
                           with the help of each and every determined mind
                           that makes us, the NOVUS.
                       </p>
                   </div>
                   <div>
                       <img src="../../assets/images/novus_logo.png" alt="">
                   </div>
               </div>
               <div class="contact__details--address">
                   <div>
                       <h3>Become a teammate</h3>
                       <p>nkpc14@gmail.com</p>
                   </div>
                   <div class="contact__details--address-bottom">
                       <h3>Address</h3>
                       <p>Lovely Professional University, Jalandhar, Punjab, 144007</p>
                   </div>

               </div>
               <div class="contact__details--team">
                   <div>
                       <h3>Our Projects</h3>
                       <p>Project 1</p>
                       <p>Project 2</p>
                       <p>Project 3</p>
                   </div>
                   <div class="contact__details--team-bottom">
                       <h3>About team member</h3>
                       <p>team@novus.com</p>
                   </div>
               </div>
               <div class="contact__details--social">
                   <div>
                       <h3>Social</h3>
                       <p>Facebook</p>
                       <p>Instagram</p>
                       <p>LinkedIn</p>
                       <p>Twitter</p>
                   </div>
               </div>
               <div class="contact__details--studio">
                   <div>
                       <h3>Studio</h3>
                       <p>Career</p>
                       <p>Insights</p>
                       <p>About Us</p>
                   </div>
               </div>
           </div>
       </div>
   </div>
    
</template>

<script>
    export default {
        name: "ContactUsSection"
    }
</script>

<style scoped lang="scss">
    .divider{
        margin: 6rem 6rem 0 6rem;
        font-family: Poppins,sans-serif;

    }
    .contact{
        font-family: Poppins,sans-serif;
        display: flex;
        justify-content: center;
        flex-direction: column;
        margin-top: 8rem;
        & h2{
            font-size: 5rem;
            max-width: 112rem;
            padding-left: 10vw;
            & span{
                color: #D9927F;
                border-bottom: solid 0.02rem #FF4E00;
            }
        }

        &__details{
            display: flex;
            margin-top: 25rem;
            justify-content: space-around;
            & h3{
                font-size: 2rem;
            }
            &--about{
                max-width: 40rem;
                display: flex;
                flex-direction: column;
                justify-content: space-between;
                & img{
                    margin-top: 6rem;
                }
            }
            &--address{
                display: flex;
                flex-direction: column;
                /*justify-content: space-between;*/

                &-bottom{
                    margin-top: 9.1rem;
                }
            }
            &--team{
                display: flex;
                flex-direction: column;
                /*justify-content: space-between;*/

                &-bottom{
                    margin-top: 4rem;
                }            }
            &--social{
                display: flex;
                flex-direction: column;
            }
            &--studio{
                display: flex;
                flex-direction: column;
            }
        }
    }

</style>
