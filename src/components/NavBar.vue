<!-- <script>
export default{
    data(){
        return{
          };
        },
        props:{
        info:Array,
      },
};
</script>

<template>
<div  v-for="(text, i) in firstList" :key="i" class="header-nav">
            <span>{{ text.minnie }}</span>
            <span>{{ text.minnie }}</span>
            <span>{{ text.minnie }}</span>   
            <span>{{ text.minnie }}</span>
            <span>{{ text.minnie }} <button>New</button></span>
            <span>{{ text.minnie }}</span>
            <span>{{ text.minnie }}</span>
            <span><i class="fa-solid fa-cart-shopping"></i></span>
        </div>
</template>

<style lang="scss">
@use '../styles/general.scss';
@use '../styles/partials/variables' as *;
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
                    padding: 0px 2px;
                }
                button:hover{
                    color: $white-color;
                }
        }
        span:hover{
            color: $white-color;
        }
    }
</style> -->
