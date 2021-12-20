<template>
    <footer>
        <div class="container">
            <div class="footer_menu">
                <div class="first_column">
                    <div>
                        <h3 v-for="(link, index) in dcComics" :key="index" > {{ link.title }} </h3>
                        <ul>
                            <li v-for="(link, index) in dcComicsLinks" :key="index">
                                <a href="">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h3 v-for="(link, index) in shop" :key="index" > {{ link.title }} </h3>
                        <ul>
                            <li v-for="(link, index) in shopLinks" :key="index">
                                <a href="">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="second_column">
                    <div>
                        <h3 v-for="(link, index) in dC" :key="index" > {{ link.title }} </h3>
                        <ul>
                            <li v-for="(link, index) in dCLinks" :key="index">
                                <a href="">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="third_column">
                    <h3 v-for="(link, index) in sites" :key="index" > {{ link.title }} </h3>
                    <ul>
                        <li v-for="(link, index) in sitesLinks" :key="index">
                            <a href="">
                                {{ link.text }}
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="crooked_logo">
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer",
    data: function() {
        return {
            dcComics: [
                {
                    title: 'DC COMICS',
                },
            ],
            dcComicsLinks: [
                {
                    text: 'Characters',
                    url: '#',
                },
                {
                    text: 'Comics',
                    url: '#',
                },
                {
                    text: 'Movies',
                    url: '#',
                },
                {
                    text: 'Tv',
                    url: '#',
                },
                {
                    text: 'Games',
                    url: '#',
                },
                {
                    text: 'Videos',
                    url: '#',
                },
                {
                    text: 'News',
                    url: '#',
                },
            ],
            shop: [
                {
                    title: 'SHOP',
                },
            ],
            shopLinks: [
                {
                    text: 'Shop Dc',
                    url: '#',
                },
                {
                    text: 'Shop Dc Collectionables',
                    url: '#',
                },
            ],
            dC: [
                {
                    title: 'DC',
                },
            ],
            dCLinks: [
                {
                    text: 'Term Of Use',
                    url: '#',
                },
                {
                    text: 'Privacy policy (New)',
                    url: '#',
                },
                {
                    text: 'Ad Choices',
                    url: '#',
                },
                {
                    text: 'Advertising',
                    url: '#',
                },
                {
                    text: 'Jobs',
                    url: '#',
                },
                {
                    text: 'Subscriptions',
                    url: '#',
                },
                {
                    text: 'talent Workshops',
                    url: '#',
                },
                {
                    text: 'CPSC Workshops',
                    url: '#',
                },
                {
                    text: 'Ratings',
                    url: '#',
                },
                {
                    text: 'Shop Help',
                    url: '#',
                },
                {
                    text: 'Contact Us',
                    url: '#',
                },
            ],
            sites: [
                {
                    title: 'SITES',
                },
            ],
            sitesLinks: [
                {
                    text: 'DC',
                    url: '#',
                },
                {
                    text: 'MAD Magize',
                    url: '#',
                },
                {
                    text: 'DC Kids',
                    url: '#',
                },
                {
                    text: 'DC Universe',
                    url: '#',
                },
                {
                    text: 'DC Power Visa',
                    url: '#',
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
footer{
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 387px;
    overflow: hidden;
}

.container{
    display: flex;
    justify-content: space-between;
}

.footer_menu{
    display: flex;
    padding: 40px 0 40px;

    &>*{
        margin: 0 15px;
    }

    a{
        color: #959595;
        font-size: 12px;
    }

    h3{
        color: white;
        margin-bottom: 15px;
    }

    .first_column{
        &>*{
            margin-bottom: 30px;
        }
    }
}

.crooked_logo{
    background-image: url('../assets/img/dc-logo-bg.png');
    height: 429px;
    width: 100%;
    background-repeat: no-repeat;
    background-position: right;
}

</style>