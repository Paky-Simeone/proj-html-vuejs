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
    <div class="right-box demos">
      <i class="fas fa-folder-open"></i>
      Demos
    </div>

    <div class="right-box on-sale">
      <p><sup class="small-size">$</sup>39</p>
      OnSale
    </div>
    
</section>
</template>

<style lang="scss">
@use '../styles/Header.scss';
@use '../styles/partials/variables' as *;
.right-box {
    position: fixed;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    cursor: pointer;
    height: 50px;
    width: 50px;
    z-index: 1010;
    border-radius: 5px;
    background-color: $white-color;
    box-shadow: 0 0 25px 5px rgb(0 0 0 / 20%);
    font-weight: 600;
    font-size: 10px;
}
.right-box.demos{
    right: 10px;
    top: 150px;
    .fa-folder-open {
        font-size: 20px;
        color: #33475b;
    }
}

.right-box.on-sale {
    right: 10px;
    top: 210px;
  p {
    font-size: 20px;
    color: #52b838;
    margin-bottom: inherit;
    .small-size {
        color: #52b838;
        font-size: 10px;
    }
  }
}

</style>
