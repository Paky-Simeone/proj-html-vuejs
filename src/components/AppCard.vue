<script>
export default{
    props:{
        item:Object,
    },
    methods:{
        generateURL(path) {
         return new URL(path, import.meta.url).href;
        },
    }
}
</script>

<template>
<div class="col-2"> 
    <div class="card border-0">
        <img :src="generateURL('../assets/img/'+ item.image)" class="card-img-top pluto" :alt="item.title">
        <div class="card-body">
            <h5 class="card-title">{{ item.title }}</h5>
            <p class="divisore"></p>
            <p class="card-text">{{ item.paragraph }}</p>
            <button class="mx-4">{{ item.bottone }}</button>
        </div>
    </div>
</div>
   


</template>

<style lang="scss">
@use '../styles/Card.scss';
</style>