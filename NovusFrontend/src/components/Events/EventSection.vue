<template>
    <div>

        <div class="divider">
            <h3>Events</h3>
            <hr>
        </div>
        <div class="events">
            <div class="events__info">
                <h3><span>Join us</span> on our live events.</h3>
                <p class="events__info">
                    We regularly keep on organising events inside our university
                    so anyone who is interested could reach us over there.
                    We’ll be really happy to assist you.
                </p>
            </div>

            <div class="events__main">
                <p class="events__main--current-event">Current event</p>
                <div class="events__main--event">
                    <div>
                        <h3>Event Title</h3>
                        <h4>Tagline for the event</h4>
                    </div>
                    <div>
                        <p>Ticket Price: <span>$5</span></p>
                    </div>
                </div>
                <p class="events__main--last">Last events</p>
                <div class="events__main--lastevents">
                    <div class="events__main--lastevents--in">
                        <h4>Event Title</h4>
                        <span>Tagline</span>
                    </div>
                    <div class="events__main--lastevents--in">
                        <h4>Event Title</h4>
                        <span>Tagline</span>
                    </div>
                    <div class="events__main--lastevents--in events__main--lastevents--in-lastIndex">
                        <h4>Event Title</h4>
                        <span>Tagline</span>
                    </div>
                </div>
                <div class="events__main--eventDetails">
                    <h4>About the event</h4>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit,
                        sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                        Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
                        nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
                        reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
                        pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
                        culpa qui officia deserunt mollit anim id est laborum.
                    </p>
                </div>
                <div class="events__main--venue">
                    <p>Venue</p>
                    <p>Lovely Professional University,
                        Punjab, 144007, IN.</p>
                </div>
                <div class="events__main--date">
                    <p>Date</p>
                    <span>Friday, June 14</span>
                </div>
                <div class="events__main--seeMore">
                    <a href="">See all events</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "EventSection"
    }
</script>

<style scoped lang="scss">
    .divider{
        margin: 15rem 6rem 0 6rem;
        font-family: Poppins,sans-serif;

    }
    .events{
        &__info{
            font-family: Poppins,sans-serif;
            & h3{
                font-size: 6rem;
                padding: 6rem;
                & span{
                    color: #FF4E00;
                }
            }

            & p{
                padding-left: 6rem;
                max-width: 66rem;
                font-size: 2rem;
            }
        }

        &__main{
            display: grid;
            margin-top: 8rem;
            padding-bottom: 4rem;
            grid-template-columns: 2fr 2fr 2fr 1fr 1fr;
            grid-template-rows: auto auto auto auto auto ;
            font-family: Poppins,sans-serif;
            &--current-event{
                grid-column: 1/4;
                grid-row: 1/2;
                display: flex;
                justify-content: center;
                /*background-color: chartreuse;*/
                font-size: 3.5rem;
                font-weight: 800;
            }
            &--event{
                grid-column: 1/4;
                grid-row: 2/4;
                background-color: #444153;
                padding: 3rem;
                height: 30rem;
                margin-left: 6rem;
                margin-right: 8rem;
                margin-top: 2rem;
                display: flex;
                align-items: end;
                justify-content: space-between;

                & h3{
                    font-size: 5rem;
                }
                & h4{
                    font-weight: 300;
                }
                & p{
                    font-weight: bold;
                }
                & span{
                    font-size: 3rem;
                    font-weight: 700;
                    color: #FF4E00;
                }
            }

            &--eventDetails{
                grid-column: 1/3;
                grid-row: 4/5;
                /*background-color: black;*/
                padding: 7rem;
                & h4{
                    font-size: 2rem;
                    margin-bottom: 1rem;
                }
            }
            &--venue{
                grid-column: 1/3;
                grid-row: 5/6;
                /*background-color: rebeccapurple;*/
                padding-left: 7rem;
            }
            &--date{
                grid-column: 3/4;
                grid-row: 5/6;
                /*background-color: green;*/
            }
            &--seeMore{
                grid-column: 4/6;
                grid-row: 5/6;
                /*background-color: red;*/
                margin-left: 30%;
                & a{
                    color: #fff;
                    border-bottom: solid 0.02rem #FF4E00;
                }
            }
            &--last{
                grid-column: 4/6;
                grid-row: 1/2;
                /*background-color: aquamarine;*/
            }
            &--lastevents{
                /*background-color: pink;*/
                grid-row: 2/5;
                grid-column: 4/6;
                &--in{
                    background-color: #444153;
                    margin: 1rem;
                    height: 16rem;
                    width: 30rem;
                    display: flex;
                    align-items: start;
                    justify-content: end;
                    padding: 2rem;
                    flex-direction: column;
                    & h4{
                        font-size: 2rem;
                    }
                    & span {
                      font-weight: 300;
                    }

                    &-lastIndex{
                        background: linear-gradient(rgba(#444153,1),rgba(#fff,0));
                    }

                }
            }
        }
    }
</style>