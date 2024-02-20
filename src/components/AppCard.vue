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
            <p class="card-text">{{ item.paragraph }}</p>
            <button><a href="#">{{ item.bottone }}</a></button>
        </div>
    </div>
</div>
   


</template>

<style lang="scss">
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
}
.card-title{
    text-align: center;
    margin-top: 1rem;
}
.card-text{
    text-align: center;
}
button{
    align-items: center;
}

</style>