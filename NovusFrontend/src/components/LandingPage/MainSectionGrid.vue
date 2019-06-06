<template>
    <div class="mainSection">

        <div class="mainSection--content">

            <h1>
                <span class="mainSection--content-novus">Novus</span>
                is a digital studio
                that develop websites and
                Mobile applications.

            </h1>

        </div>
        <div class="mainSection--arts">
            <img class="mainSection--arts-semi_cir_empty" src="../../assets/images/semi_cir_empty.png" alt="">
            <img class="mainSection--arts-semi_cir_fill" src="../../assets/images/semi_cir_fill.png" alt="">
            <img class="mainSection--arts-rectangle" src="../../assets/images/rectangle.png" alt="">
            <img class="mainSection--arts-Ellipse" src="../../assets/images/Ellipse.png" alt="">
            <img class="mainSection--arts-dots" src="../../assets/images/dots.png" alt="">
        </div>



        <div class="mainSection--scroll">
            <p>
                NOVUS is a student organisation since 2017 led by aspiring minds. We are pushing its limits
                with the help of each and every determined mind that makes us, the NOVUS.
            </p>
            <div class="mainSection--scroll-in">
                <p>Scroll to see more</p>
                <img src="../../assets/images/Arrow.png" alt="">
            </div>
        </div>

        <div class="mainSection--photo">
            <p>
                Innovation drives us and we are hunting for it; hunting hunting for people who stand
                out in crowd, like you.
            </p>

            <a href="">View Photos / videos</a>

        </div>

        <div class="mainSection--video">

            <img src="../../assets/images/video.png" alt="">
        </div>
        </div>
</template>

<script>
    import Header from './Header'
    export default {
        name: "MainSectionGrid",
        components:{
            Header
        }
    }
</script>

<style scoped lang="scss">

  .mainSection{
      display: grid;
      grid-template-columns: auto  auto auto auto auto;
      grid-template-rows: auto auto;
      padding: 6rem;
      font-family: Poppins,sans-serif;
      grid-row-gap: 15rem;
      grid-column-gap: 13rem;

      &--content{
          grid-column: 1/4;
          grid-row: 1/2;
          padding: 2rem;
          font-size: 2.9rem;
          &-novus{
              border-top:solid 0.2rem #FF4E00;
          }
      }

      &--arts{
          position: relative;
          grid-column:4/6;

          & img{

          }

          &-semi_cir_empty{
              transform: translate(15rem,-6rem);
          }
          &-semi_cir_fill{
              transform: translate(1rem,5rem);
          }
          &-rectangle{
                transform: translate(5rem,15rem);
          }
          &-Ellipse{
            transform: translate(-23rem,5rem);
          }
          &-dots{
            transform: translate(40rem,-12rem);
          }
      }

      &--scroll{
          grid-row:2/3;
          grid-column:1/3;
          display: flex;
          justify-content: space-between;
          flex-direction: column;
          font-size: 1.8rem;
          padding: 3rem;
          &-in{
              display: flex;
          }
      }

      &--photo{
          grid-row:2/3;
          grid-column:3/5;
          display: flex;
          justify-content: space-between;
          align-items: end;
          flex-direction: column;
          font-size: 1.8rem;
          padding: 3rem;

          & a{
              color: #fff;
              border: solid 0.02rem #FF4E00;
              padding: 1rem 2rem;
          }
      }

      &--video{
          grid-column:5/6;
          padding: 1rem;

      }
  }
</style>