<template>
    <div class="new_arrivals">
        <h1 class="title">New Arrivals</h1>
            <div class="billboard">
                <el-carousel trigger="click" height="600px" type="card" interval="6000">
                    <el-carousel-item v-for="item in list" :key="item">
                        <h3 class="slogan">piggy market</h3>
                    </el-carousel-item>
                </el-carousel>
            </div>
    </div>
</template>

<script>
    export default {
        name: "NewArrivals",
        data() {
            return {
                list: ["a", "b", "c", "d", "e", "f", "g"]
            }
        }
    }
</script>

<style scoped>
    .new_arrivals {
        font-family: 'CGB';
        height: 800px;
        margin-left: 100px;
        margin-right: 100px;
    }

    .title {
        text-align: left;
    }

    .el-carousel__item h3 {
        color: #475669;
        font-size: 14px;
        opacity: 0.75;
        line-height: 500px;
        margin: 0;
    }

    .el-carousel__item:nth-child(4n) {
        background: url("../assets/background2.jpg") no-repeat fixed ;
        background-size: inherit;
    }

    .el-carousel__item:nth-child(4n+1) {
        background: url("../assets/background1.jpg") no-repeat fixed;
        background-size: inherit;
    }

    .el-carousel__item:nth-child(4n+2) {
        background: url("../assets/background3.png") no-repeat fixed;
        background-size: inherit;
    }

    .el-carousel__item:nth-child(4n+3) {
        background: url("../assets/background4.png") no-repeat fixed;
        background-size: inherit;
    }
</style>