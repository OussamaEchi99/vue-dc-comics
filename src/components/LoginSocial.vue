<template>
    <div class="login_social">
        <div class="container">
            <div class="login">
                <a href="#">
                    SIGN-UP NOW!
                </a>
            </div>
            <div class="social">
                <ul>
                    <li><h2>FOLLOW US</h2></li>
                    <li v-for="(link, index) in social" :key="index">
                        <a href="">
                            <img :src="require('../assets/img/footer-' + link.imgScr + '.png')" alt="">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "LoginSocial",
    data: function() {
        return {
            social: [
                {
                    imgScr: 'facebook',
                    url: '#',
                },
                {
                    imgScr: 'twitter',
                    url: '#',
                },
                {
                    imgScr: 'youtube',
                    url: '#',
                },
                {
                    imgScr: 'pinterest',
                    url: '#',
                },
                {
                    imgScr: 'periscope',
                    url: '#',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/Variables';

.login_social{
    background-color: #303030;
    z-index: 1;
}

.container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 45px 0;
}

.login{
    a{
        color: white;
        border: 2px solid $brand_primary_color;
        padding: 15px;
    }
}

.social{


    ul{
        display: flex;
        align-items: center;
    }

    li{

        margin: 0 10px;

        &:first-child{
            color: $brand_primary_color;
            margin: 0 25px;
        }
    }
}
</style>
