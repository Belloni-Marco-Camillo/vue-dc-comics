<template>
    <div class="jumbotron-dc">
        
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
    .jumbotron-dc{
        background-image: url(./../assets/img/jumbotron.jpg);
        background-size:cover;
        background-repeat: no-repeat;
        height: 500px;
    }
</style>