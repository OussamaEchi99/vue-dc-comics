<template>
    <div class="pre_footer">
        <div class="container">
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url">
                        <div>
                            <img :src="require('../assets/img/buy-comics-' + link.image)" alt="">
                        </div>

                        <div>
                            <span> {{ link.text }} </span>
                        </div>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: "PreFooter",
    data: function() {
        return {
            links: [
                {
                    text: 'DIGITAL COMICS',
                    url: '#',
                    image: 'digital-comics.png'
                },
                {
                    text: 'DC MERCHANDISE',
                    url: '#',
                    image: 'dc-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    url: '#',
                    image: 'subscription.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    url: '#',
                    image: 'shop-locator.png'
                },
                {
                    text: 'DC POWER VISA',
                    url: '#',
                    image: 'dc-power-visa.svg'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

.pre_footer{
    height: 150px;
    background-color: $brand_primary_color;
}
</style>