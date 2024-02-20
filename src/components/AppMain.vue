<script>
import AppCard from './AppCard.vue';
export default{
    data(){
        return{
            pippos:[
            {
                image:"sushi-1.png",
                title:"THE BEST TABLE IN TOWN",
                paragraph:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit earum voluptates quod dolore, accusantium, natus quos eveniet consequatur quae sit maiores dignissimos fugit illum veritatis. Optio ea veritatis doloremque vel.",
                bottone:"EXPLORE THE MENU",
            },
            {
                image:"sushi-2.png",
                title:"PERFECT FOR GROUPS",
                paragraph:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit earum voluptates quod dolore, accusantium, natus quos eveniet consequatur quae sit maiores dignissimos fugit illum veritatis. Optio ea veritatis doloremque vel.",
                bottone:"MAKE A RESERVATION",
            },
            {
                image:"sushi-3.png",
                title:"FRESH PRODUCE EVERYDAY",
                paragraph:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit earum voluptates quod dolore, accusantium, natus quos eveniet consequatur quae sit maiores dignissimos fugit illum veritatis. Optio ea veritatis doloremque vel.",
                bottone:"LEARN MORE ABOUT US",
            },
            ],
        };
    },
    

    components:{AppCard},
};
</script>

<template>
    <!-- PRIMA SECTION -->
<section class="firstsection">
    <div class="leftfirstsection">
        <p><strong>HAC TELLUS, FELIS RISUS AT</strong> mattis mattis. Eget euismod semper eget tortor, donec amet, blandit. Tristique facilisi faucibus elementum feugiat in nam in feugiat. Ipsum odio etam duis facilisis amet vulputate.</p>
        <h1>FOOD IS OUR COMMON GROUND, A UNIVERSAL EXPERIENCE.</h1>
        <p>Tristique tempus condimentum diam donec. Condimentum ullamcorper sit elementum hendrerit mi nulla in consequat, ut. Metus, nullam scelerisque netus viverra dui.</p>
        <img src="../assets/img/signature-200x172.jpg" alt="">
    </div>
    <div class="rightfirstsection">
        <div class="right_img_firstsection">
            <img src="../assets/img/info22x.jpg" alt="">
            <p>CALIFORNIA ROLLS - $22</p>
        </div>
    </div>
    
</section>
<!-- SECONDA SECTION -->
<section class="secondsection">
    <div class="centralfsecondsection">
        <div class="row justify-content-center mt-5">
            <AppCard v-for="pippo in pippos" :item="pippo"></AppCard>
        </div>
    </div>
</section>
<!-- TERZA SECTION -->
<section class="thirdsection">
    <div class="leftthirdsection">
        <img src="../assets/img/slider32x.jpg" alt="">
    </div>
    <div class="rightthirdsection">
        <div class="jumbo-text-up">
            <p class="linea"></p>
            <p>FINE DINING EXPIRIENCE</p>
        </div>
        <div class="jumbo-text-down">
            <h1>THE BEST TABLE IN <br/>TOWN</h1>
            <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
            <button>EXPLORE THE MENU</button>
        </div>
    </div>
</section>
<!-- QUARTA SECTION -->
<section class="quartasection">
    <H2>What critics are saying about us</H2>
    <p class="divisore_centrale"></p>
    <div class="cardcentrale">
        <div class="leftcardcentrale">
            <img src="" alt="">
        </div>
        <div class="rightcardcentrale"></div>
    </div>
    
</section>
    
</template>

<style lang="scss">
@use '../styles/general.scss';
@use '../styles/partials/variables' as *;

.firstsection{
    background-color: $white-color;
    display: flex;

    // Parte Sinistra Prima Section
        .leftfirstsection{
            width: 50%;
            margin-left: 10.5rem;
            margin-top: 10rem;
            p{
                width: 28rem;
            }
            h1{
                width: 36rem;
                margin: 1.5rem 0rem;
                font-size: xxx-large;
            }
            img{
                margin-top: 1.5rem;
                width: 150px;
                height: 150px;
            }
            
        }

    // Parte Destra Prima Section
    .rightfirstsection{
        width: 50%;
        margin-top: 7rem;
        margin-right: 8.5rem;
        margin-left: 2rem;
        .right_img_firstsection{
            img{
                position: absolute;
                width: 35rem;
                height: 40rem;
            }
            img:hover{
                box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
                cursor: pointer;
                width: 36rem;
                height: 41rem;
            }
            p{
                position: relative;
                color: white;
                top: 37rem;
                left: 12.5rem;
            }
        }
    }
}
// Parte Centrale Seconda Section
.centralsecondsection{
    display: flex;
    justify-content: center;
    margin-top: 4rem;
}
// TERZA SECTION
.thirdsection{
    display: flex;
    height: 60vh;
    margin-top: 3rem;
    .leftthirdsection{
        width: 60%;
        img{
            width: 100%;
            height: 60vh;
            object-fit: cover;
        }
    }
    .rightthirdsection{
        background-color: $black-color;
        width: 40%;
        .jumbo-text-up{
                margin-top: 3rem;
                margin-left: 6rem;
                display: flex;
                align-items: center;
                    .linea{
                        border: 1px solid $gray-color;
                        border-radius: 2px;
                        background-color: $gray-color;
                        width: 40px;
                        height: 3px;
                        margin-right: 2rem;
                    }
                    p{
                        color: $gray-color;
                    }
            }
            .jumbo-text-down{
                margin-top: 3rem;
                margin-left: 10.5rem;
                h1{
                    color: $white-color;
                    font-size: xxx-large;
                }
                p{
                    color: $gray-color;
                    margin-top: 3rem;
                    font-size: large;
                    width: 20rem;
                }
                button{
                    border: 1px solid $gray-color;
                    color: $gray-color;
                    background: none;
                    padding: 15px;
                    margin-top: 2rem;
                }
                button:hover{
                    cursor: pointer;
                    color: $black-color;
                    background-color: $white-color;
                }
            }
    }

}
// QUARTA SECTION
.quartasection{
    H2{
    font-family: italic;
    text-align: center;
    margin-top: 3rem;
    margin-bottom: 1.5rem;
    }
    .divisore_centrale{
        margin-left: 56rem;
        text-align: center;
        border: 1px solid $gray-color;
        border-radius: 2px;
        background-color: $gray-color;
        width: 100px;
        height: 3px;
    }
    .cardcentrale{
        display: flex;
        width: 1200px;
        .leftcardcentrale{
            width: 50%;
        }
        .rightcardcentrale{
            width: 50%;
        }
    }
}
</style>