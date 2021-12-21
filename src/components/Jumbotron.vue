<template>
    <div class="jumbotron">
        <div class="container">
            <div class="title">
                <h2>CURRENT SERIES</h2>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

.jumbotron{
    width: 100%;
    height: 500px;
    background-image: url('../assets/img/jumbotron.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
}

.container{
    display: flex;
    align-items: flex-end;
    height: 100%;

    .title{

        h2{
        position: absolute;
        color: white;
        background-color: $brand_primary_color;
        padding: 10px 30px;
        bottom: -25px;
        }
    }
}
</style>