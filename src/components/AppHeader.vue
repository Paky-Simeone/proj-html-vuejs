<script>
export default{
}
</script>

<template>
<section class="header-section">
    <div class="left">
        <div>
            <img src="../assets/img/logo-restaurant-2x-200x38.png" alt="">
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
@use '../styles/general.scss';
.header-section{
    display: flex;
    .left{
        width: 40%;
        background-color: black;
        height: 100vh;
        img{
            cursor: pointer;
        }
    }
}
.right{
    width: 60%;
    height: 4rem;
    img{
        position: absolute;
        width: 60%;
        height: 100%;
        object-fit: cover;
    }
    .header-nav{
        margin-top: 3rem;
        margin-right: 8.5rem;
        position: relative;
        display: flex;
        justify-content: right;
        span{
            margin-right: 50px;
            color: lightgrey;
            cursor: pointer;
                button{
                    border: 1px solid white;
                    border-radius: 2px 2px;
                    background-color: none;
                    color: white;
                    cursor: pointer;
                }
        }
        span:hover{
            color: white;
        }
    }
}  
</style>
