<script>
export default{
}
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
            <h1>FINE DINING EXPIRIENCE</h1>
            <p>Pellentesqye vitae viverra risus, sagittis. Venenatis ridiculus scelerisque nisi in urna nulla. Sit tempor a et nisl, ac felis.</p>
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
@use '../styles/general.scss';
@use '../styles/partials/variables' as *;
.header-section{
    display: flex;
    .left{
        width: 40%;
        background-color: $black-color;
        height: 80vh;
            img{
                margin-top: 3rem;
                margin-left: 6rem;
                cursor: pointer;
            }
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
.right{
    width: 60%;
    height: 80vh;
    img{
        position: absolute;
        width: 60%;
        height: 80vh;
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
            color: $gray-color;
            cursor: pointer;
                button{
                    border: 1px solid $white-color;
                    border-radius: 2px 2px;
                    background: none;
                    color: $gray-color;
                    cursor: pointer;
                }
                button:hover{
                    color: $white-color;
                }
        }
        span:hover{
            color: $white-color;
        }
    }
}  
</style>
