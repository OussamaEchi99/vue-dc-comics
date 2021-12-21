<template>
    <a href="#" class="product">
        <div class="image">
            <img :src="productListObject.thumb" alt="">
        </div>
        <span>{{productListObject.series}}</span>
    </a>
</template>

<script>
export default {
    name: 'Product',
    props: ['productListObject'],
}
</script>

<style lang="scss" scoped>
.product{
    width: calc(( 100% / 6 ));
    display: block;
    color: white;
    margin-bottom: 50px;

    .image{
        height: 200px;
        overflow: hidden;
        margin-bottom: 20px;   
        img{
            width: auto;
        }
    }
}
</style>