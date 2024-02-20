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
<section class="secondsection">
    <div class="centralfsecondsection">
        <div class="row justify-content-center mt-5">
            <AppCard v-for="pippo in pippos" :item="pippo"></AppCard>
        </div>
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
                width: 37rem;
                height: 42rem;
            }
            p{
                position: relative;
                color: white;
                top: 37rem;
                left: 12.5rem;
            }
        }
    }
    // Parte Centrale Seconda Section
    .centralsecondsection{
        display: flex;
        justify-content: center;
        margin-top: 4rem;
    }
}
</style>