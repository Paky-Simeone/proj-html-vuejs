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
    <div class="d-flex justify-content-center">
        <div class="cardcentrale">
            <div class="leftcardcentrale">
                <img src="../assets/img/blog72x-600x687.jpg" alt="">
            </div>
            <div class="rightcardcentrale">
                <p class="namestewert">Meggy Stewert</p>
                <h2 class="titlenytimes">NEW YORK TIMES</h2>
                <p class="star"><i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i></p>
                <p class="linea"></p>
                <p class="textcardcentrale">Non arcu mauris tortor ultrices mollis tellus <br/> eusimod fermentum. Habitant amet tincidunt <br/> id sapien accumsan sed at. <br/> <br/>Mmalesuada ullamcorper amet. Pretium<br/> pretium dignissim nisi.</p>
                <button>READ FULL ARTICLE</button>
            </div>
        </div>
    </div>
    <div class="d-flex justify-content-center">
        <div class="cardcentraleleft">
            <p class="namestewert">Mary Maxey</p>
                <h2 class="titlenytimes">THE GUARDIAN</h2>
                <p class="star"><i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i></p>
                <p class="linea"></p>
                <p class="textcardcentrale">Non arcu mauris tortor ultrices mollis tellus <br/> eusimod fermentum. Habitant amet tincidunt <br/> id sapien accumsan sed at. </p>
                <button>READ FULL ARTICLE</button>
        </div>
        <div class="cardcentraleright">
            <p class="namestewert">Patrick Monroe</p>
                <h2 class="titlenytimes">GLOBE AND MAIL</h2>
                <p class="star"><i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i> <i class="fa-solid fa-star"></i></p>
                <p class="linea"></p>
                <p class="textcardcentrale">Non arcu mauris tortor ultrices mollis tellus <br/> eusimod fermentum. Habitant amet tincidunt <br/> id sapien accumsan sed at. </p>
                <button>READ FULL ARTICLE</button>
        </div>
    </div>
</section>

<!-- QUINTA SECTION -->
<section class="quintasection">
        <p>KUNG PAO CHICKEN - $32</p>
</section> 

<!-- SESTA SECTION -->
<section class="sestasection">
    <h2>Latest News & promotions</h2>
    <p class="divisore_centrale"></p>

    <!-- box news x3 -->
    <div class="news-container d-flex space-between">
      <div class="news-card">
        <img src="../assets/img/blog92x.jpg" alt="" />
        <div class="overlay"></div>
        <div class="news-card-text">
          <i class="fas fa-link"></i>
          <h2>THE BEST COFFEE IN TOWN</h2>
          <p>News</p>
        </div>
        <div class="box-hide">
          <h2 class="text-box">THE BEST COFFEE IN TOWN</h2>
          <p>By admin | January 7th, 2020 | Categories: News</p>
        </div>
      </div>

      <div class="news-card">
        <img src="../assets/img/blog72x-600x687.jpg" alt="" />
        <div class="overlay"></div>
        <div class="news-card-text">
          <i class="fas fa-link"></i>
          <h2>DISCOVER OUR NEW MENU</h2>
          <p>News</p>
        </div>
        <div class="box-hide">
          <h2 class="text-box">DISCOVER OUR NEW MENU</h2>
          <p>By admin | January 7th, 2020 | Categories: News</p>
        </div>
      </div>

      <div class="news-card">
        <img src="../assets/img/blog82x.jpg" alt="" />
        <div class="overlay"></div>
        <div class="news-card-text">
          <i class="fas fa-link"></i>
          <h2>WE NOW ACCEPT SQUARE!</h2>
          <p>News</p>
        </div>
        <div class="box-hide">
          <h2 class="text-box">WE NOW ACCEPT SQUARE!</h2>
          <p>By admin | January 7th, 2020 | Categories: News</p>
        </div>
      </div>
    </div>
</section>

<!-- SETTIMA SECTION -->
<section class="settimasection">
</section>

</template>

<style lang="scss">
@use '../styles/main.scss';
@use '../styles/partials/variables' as *;
</style>