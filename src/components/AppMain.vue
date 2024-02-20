<script>
export default{
    
}
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
        margin-right: 10.5rem;
        .right_img_firstsection{
            
        }
    }
}
</style>