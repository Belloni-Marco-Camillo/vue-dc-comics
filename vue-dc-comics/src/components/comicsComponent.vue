<template>
    
    <div class="card-dc col-2 text-white">
        <img :src="img">
        <div class="offset-2 col-8 text-center">{{title}}</div>
    </div>
</template>


<script>
export default {
    name: "comicisComponent",
    props:{
        img:String,
        title: String,
    },
}
</script>

<style lang="scss">
.card-dc{
    text-align: center;
    background-color: $primaryColor;
    img{
        height: 190px;
        width: 190px;
    }

}

</style>