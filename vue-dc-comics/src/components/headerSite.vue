<template>
    <header>
        <div class="container d-flex justify-content-between align-items-center">
            <div>
                <img src="./../assets/img/dc-logo.png" alt="">  
            </div>
            <div>
                <a :href="item.href" v-for="item in menu" :key="item.id"> {{item.text}}</a>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'headerSite',
    data(){
        return{
            menu: [
                {
                    id:1,
                    href: "#",
                    text: "characters",
                },
                {
                    id:2,
                    href: "#",
                    text: "comics",
                },
                {
                    id:3,
                    href: "#",
                    text: "movies",
                },
                {
                    id:4,
                    href: "#",
                    text: "tv",
                },
                {
                    id:5,
                    href: "#",
                    text: "games",
                },
                {
                    id:6,
                    href: "#",
                    text: "collectibles",
                },
                {
                    id:7,
                    href: "#",
                    text: "videos",
                },
                {
                    id:8,
                    href: "#",
                    text: "fans",
                },
                {
                    id:9,
                    href: "#",
                    text: "news",
                },
                {
                    id:10,
                    href: "#",
                    text: "shop",
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '~@/assets/scss/style.scss';
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
a{
    margin: 0 20px;
    color: black;
    text-decoration: none;
}
    
</style>

