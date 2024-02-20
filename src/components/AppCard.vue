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
@use '../styles/general.scss';
@use '../styles/partials/variables' as *;
.card{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 200px;
    width: 300px;
    .pluto{
        width: 70px;
        height: 70px;
    }
    .pluto:hover{
        cursor: pointer;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    }
}
.card-title{
    text-align: center;
    margin-top: 1rem;
}
.divisore{
    text-align: center;
    border: 1px solid $gray-color;
    border-radius: 2px;
    background-color: $gray-color;
    width: 100px;
    height: 3px;
    margin-left: 5rem;
    margin-top: 1.2rem;
}
.card-text{
    text-align: center;
}
button{
    border: 1px solid $gray-color;
    color: $gray-color;
    background: none;
    padding: 15px;
}
button:hover{
    cursor: pointer;
    border: 1px solid $black-color;
    color: $black-color;
    background-color: $white-color;
}

</style>