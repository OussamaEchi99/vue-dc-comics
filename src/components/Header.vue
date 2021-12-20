<template>
    <header>
        <div class="container">
            <div class="image">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="nav">
                <ul>
                    <li v-for="(link, index) in links" :key="index" :class="{ 'current': link.current }">
                        <a :href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </div>

        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data: function() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false
                }
            ],
        };
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

.container{
    display: flex;
    justify-content: space-between;
}

.image{
    margin: 20px 0;

    img{
        width: auto;
    }
}

.nav{

    ul{
        display: flex;
        justify-content: space-between;
        align-items: stretch;
        height: 100%;

        li{
            margin: 0 20px;
            display: flex;
            align-items: center;
            cursor: pointer;

            &.current {
                border-bottom: 5px solid $brand_primary_color;
                a{
                    color: $brand_primary_color;
                }
            }

            &:hover {
                border-bottom: 5px solid $brand_primary_color;
                a{
                    color: $brand_primary_color;
                }
            }

            a{
                color: #464646;
            }
        }
    }
}

</style>