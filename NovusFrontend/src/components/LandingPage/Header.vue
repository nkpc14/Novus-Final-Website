<template>
    <div class="header">
              <div class="header--logo">
                    <router-link class="animated bounce lightSpeedIn " to="/"><img src="../../assets/images/novus_logo.png" alt=""></router-link>
              </div>
        <div
            class="header--menu animated fadeInUp">
            <router-link to="">About</router-link>
            <router-link to="">Approach</router-link>
            <router-link to="">Team</router-link>
            <router-link to="">Events</router-link>
            <router-link to="">Projects</router-link>
            <router-link to="">Contact Us</router-link>
            <router-link to="">Sign in</router-link>
            <router-link class="animated fadeInDown slow" id="reg" to="">Register</router-link>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Header",
        data(){
          return{
          show:true
          }
        }
    }
</script>

<style scoped lang="scss">

    .header{
        /*background-color: red;*/
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 8rem;
        &--logo{
            display: flex;
            align-items: center;
            & img {
                height: 4rem;
                /*margin-top: 2rem;*/
                margin-left: 5rem;
            }
        }

        &--menu{
            /*padding-top: 2.8rem;*/
            padding-right: 5rem;
            display: flex;
            font-family: Poppins;
            justify-content: space-between;
            & a{
                color: #fff;
                margin-right: 2rem;

            }
            & #reg{
                /*background-color: red;*/
                padding:0.4rem 2rem;
                margin-top: -0.4rem;
                border: solid #FF4E00 0.01rem;
            }
        }
    }
</style>
