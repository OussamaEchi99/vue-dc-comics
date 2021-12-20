<template>
    <div class="pre_footer">
        <div class="container">
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url">
                        <div class="image">
                            <!-- <img :src="require('../assets/img/buy-comics-' + link.image)" :alt="link.text + 'Logo'"> -->
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
                    image: 'merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    url: '#',
                    image: 'subscriptions.png'
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
    .container{
        height: 100%;
        
        ul{
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;

            a{
                display: flex;
                align-items: center;
            }
        }
    }
}

.image{
    display: flex;
    justify-content: center;

   img{
        max-width: 50%;
        display: flex;
   }
}
</style>