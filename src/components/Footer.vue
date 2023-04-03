<template>
    <div class="footer">
        <el-row :gutter="20">
            <el-col :span="6">
                <div class="title">Information</div>
                <div class="detail">about piggy market</div>
                <div class="detail">responsibility</div>
                <div class="detail">size guide</div>
                <div class="detail">retailers</div>
            </el-col>
            <el-col :span="6">
                <div class="title">Custom Service</div>
                <div class="detail">contract us</div>
                <div class="detail">cookie policy</div>
                <div class="detail">faq</div>
            </el-col>
            <el-col :span="6">
                <div class="title">Social Media</div>
                <div class="detail">facebook</div>
                <div class="detail">instagram</div>
                <div class="detail">pinterest</div>
                <div class="detail">tiktok</div>
            </el-col>
            <el-col :span="6">
                <div class="title">Support</div>
                <div class="detail"><path fill="#FFF" d="M150.698 3.532l1.672.003c.452.003.905.008 1.36.02.793.022 1.719.065 2.583.22.75.135 1.38.34 1.984.648a6.392 6.392 0 0 1 2.804 2.807c.306.6.51 1.226.645 1.983.154.854.197 1.783.218 2.58.013.45.019.9.02 1.36.005.557.005 1.113.005 1.671v76.318c0 .558 0 1.114-.004 1.682-.002.45-.008.9-.02 1.35-.022.796-.065 1.725-.221 2.589a6.855 6.855 0 0 1-.645 1.975 6.397 6.397 0 0 1-2.808 2.807c-.6.306-1.228.511-1.971.645-.881.157-1.847.2-2.574.22-.457.01-.912.017-1.379.019-.555.004-1.113.004-1.669.004H14.801c-.55 0-1.1 0-1.66-.004a74.993 74.993 0 0 1-1.35-.018c-.744-.02-1.71-.064-2.584-.22a6.938 6.938 0 0 1-1.986-.65 6.337 6.337 0 0 1-1.622-1.18 6.355 6.355 0 0 1-1.178-1.623 6.935 6.935 0 0 1-.646-1.985c-.156-.863-.2-1.788-.22-2.578a66.088 66.088 0 0 1-.02-1.355l-.003-1.327V14.474l.002-1.325a66.7 66.7 0 0 1 .02-1.357c.022-.792.065-1.717.222-2.587a6.924 6.924 0 0 1 .646-1.981c.304-.598.7-1.144 1.18-1.623a6.386 6.386 0 0 1 1.624-1.18 6.96 6.96 0 0 1 1.98-.646c.865-.155 1.792-.198 2.586-.22.452-.012.905-.017 1.354-.02l1.677-.003h135.875"></path></div>
                <div class="detail">instagram</div>
                <div class="detail">pinterest</div>
                <div class="detail">tiktok</div>
            </el-col>
        </el-row>
        <div class="copyright">Copyright © 2023 Piggy Market</div>
    </div>
</template>

<script>
    export default {
        name: "Footer"
    }
</script>

<style scoped>
    .footer {
        margin-top: 100px;
        background-color: whitesmoke;
        font-family: 'CGB';
        height: 280px;
    }

    .title {
        font-size: 40px;
        margin-left: 100px;
        text-align: left;
    }

    .detail {
        font-size: 25px;
        font-family: 'CGL';
        margin-left: 100px;
        text-align: left;
        margin-top: 5px;
    }

    .copyright {
        margin-top: 50px;
    }
</style>