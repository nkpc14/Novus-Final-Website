<template>
   <div>
       <div class="divider">
           <h3>Projects</h3>
           <hr>
       </div>
       <div class="projects">
           <div class="projects__top">
               <h2>Look at all the projects that we
                   have <span>accomplished.</span></h2>
           </div>
           <div class="projects__middle">
               <hr/>
               <div class="projects__middle--project">
                   <div class="project__middle--project-div">
                       <img src="" alt="">
                   </div>
                   <h3>Google</h3>
                   <p>Project 1</p>
               </div>
               <hr/>
               <div class="projects__middle--project">
                   <div class="project__middle--project-div">
                       <img src="" alt="">
                   </div>
                   <h3>Zomato</h3>
                   <p>Project 2</p>
               </div>
               <hr/>
               <div class="projects__middle--project">
                   <div class="project__middle--project-div">
                       <img src="" alt="">
                   </div>
                   <h3>Amazon</h3>
                   <p>Project 3</p>
               </div>
               <hr/>
           </div>
           <div class="projects__bottom">
               <p>View Corner</p>
               <div>
                   <span>Study</span>
                   <img src="../../assets/images/arrow_hori.png" alt="">
               </div>
           </div>
       </div>
   </div>

</template>

<script>
    export default {
        name: "ProjectsSection"
    }
</script>

<style scoped lang="scss">
    .divider{
        margin: 15rem 6rem 0 6rem;
        font-family: Poppins,sans-serif;

    }
    .projects{
        display: flex;
        flex-direction: column;
        font-family: Poppins,sans-serif;
        padding: 6rem;
        &__top{
            & h2{
                font-size: 4rem;
                max-width: 70rem;
                & span{
                    color: #FF4E00;
                }
            }
        }

        &__middle{
            display: flex;
            justify-content:center;
            flex-wrap: wrap;
            margin-top: 8rem;
            margin-bottom: 5rem;
            & hr{
                border: 0;
                background-image: linear-gradient(180deg,transparent, #B5B1D3, transparent);
                width: 0.1rem;
            }
            &--project{
                padding: 2rem;
                /*border-left: solid 0.01rem rgba(#fff,0.2);*/
                /*border-right: solid 0.01rem rgba(#fff,0.2);*/
                width: 26vw;
                display: flex;
                flex-direction: column;

                &>div{
                    width: 100%;
                    background-color: #444153;
                    height: 40rem;
                    margin-bottom: 4rem;
                }
                & h3{
                    padding-left: 1rem;
                    font-size: 4rem;
                }
                & p{
                    padding-left: 1rem;
                    font-size: 3rem;
                    font-weight: 300;
                }
            }
        }

        &__bottom{
            padding: 4rem;
            & > div{
                display: flex;
                & img{
                    margin-left: 2rem;
                }
            }
        }
    }
</style>