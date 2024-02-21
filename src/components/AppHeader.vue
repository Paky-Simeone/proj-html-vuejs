<script>
export default{
        // props:{
        //     info:Object,
        // },
};
</script>

<template>
<section class="header-section">
    <div class="left">
        <div>
            <img src="../assets/img/logo-restaurant-2x-300x58.png" alt="">
        </div>
        <div class="jumbo-text-up">
            <p class="linea"></p>
            <p>THE BEST TABLE IN TOWN</p>
        </div>
        <div class="jumbo-text-down">
            <h1>FINE DINING <br/> EXPIRIENCE</h1>
            <p>Pellentesque vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
            <button>EXPLORE THE MENU</button>
        </div>
    </div>
    
    <div class="right">
        <img src="../assets/img/slider52x.jpg" alt="">
        <div class="header-nav">
            <span>Home</span>
            <span>Culinary History</span>
            <span>Our Team</span>   
            <span>Our Menù</span>
            <span>Take Out <button>New</button></span>
            <span>Bulletin</span>
            <span>Reservation</span>
            <span><i class="fa-solid fa-cart-shopping"></i></span>
        </div>
    </div>
    
</section>
</template>

<style lang="scss">
@use '../styles/Header.scss';
</style>
