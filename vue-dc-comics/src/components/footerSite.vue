<template>
    <footer>
        <div class="container d-flex">
            <div class="col-6 d-flex mt-5">
                <div class="col-3 text-white" v-for="({titles, links}, index) in footerMenu" :key="index" >
                    <h4 class="text-white">{{titles}}</h4>
                        <ul class="">
                            <li v-for="(link,index) in links" :key="index">
                                <a :href="link.href">{{link.text}}</a>
                            </li>
                        </ul>
                </div>
            </div>
            <div class="col-6 logo-dc">
                <img src="./../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'footerSite',
    props: {
        msg: String
    },
    data() {
        return {
            footerMenu: [
                {
                    titles: "DC Comics",
                    links: [
                        {
                            href: "#",
                            text: "Characters",
                        },
                        {
                            href: "#",
                            text: "Comics",
                        },
                        {
                            href: "#",
                            text: "Movie",
                        },
                        {
                            href: "#",
                            text: "TV",
                        },
                        {
                            href: "#",
                            text: "Games",
                        },
                        {
                            href: "#",
                            text: "Videos",
                        },
                        {
                            href: "#",
                            text: "News",
                        }
                    ]
                },
                {
                    titles: "DC",
                    links: [
                        {
                            href: "#",
                            text: "Terms of Use",
                        },
                        {
                            href: "#",
                            text: "Privacy policy (New)",
                        },
                        {
                            href: "#",
                            text: "Ad Choise",
                        },
                        {
                            href: "#",
                            text: "Advertising",
                        },
                        {
                            href: "#",
                            text: "Jobs",
                        },
                        {
                            href: "#",
                            text: "Subscription",
                        },
                        {
                            href: "#",
                            text: "Talent Workshops",
                        },
                        {
                            href: "#",
                            text: "CPSC Certificates",
                        },
                        {
                            href: "#",
                            text: "Rating",
                        },
                        {
                            href: "#",
                            text: "Shop Help",
                        },
                        {
                            href: "#",
                            text: "Contact Us",
                        }
                    ]
                },
                {
                    titles: "Sites",
                    links: [
                        {
                            href: "#",
                            text: "DC",
                        },
                        {
                            href: "#",
                            text: "MAD Magazine",
                        },
                        {
                            href: "#",
                            text: "DC Kids",
                        },
                        {
                            href: "#",
                            text: "DC Universe",
                        },
                        {
                            href: "#",
                            text: "DC Power Visa",
                        }
                    ]
                },
                {
                    titles: "Shop",
                    links: [
                        {
                            href: "#",
                            text: "Shop DC",
                        },
                        {
                            href: "#",
                            text: "Shop DC Collectibles",
                        }
                    ]
                }
            ]
        };
    }
}
</script>

<style scoped lang="scss">
footer{
    background-image: url(./../assets/img/footer-bg.jpg);
    background-size: cover;
}
li{
    color: gray;
    list-style: none;
    &:hover{
        color: #0282F9;
    }
}
.col-6{
    img{
        position: relative;
        transform: translate(0 , -15%);
    }
    height: 370px;
}


</style>