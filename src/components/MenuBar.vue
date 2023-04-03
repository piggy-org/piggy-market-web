<template>
    <div id="menubar">
        <div id="menubarLeft">
            <a href="#"><img id="logo" src="../assets/logo.png"></a>
            <a href="#"><img id="name" src="../assets/piggy_market.png" /></a>
        </div>

        <div id="menubarRight">
            <a href="#"><img id="search" src="../assets/search.png" /></a>
            <a href="#"><img id="cart" src="../assets/cart.png" /></a>
            <a href="#"><img id="user" src="../assets/user.png" /></a>
        </div>
    </div>
</template>

<script>
    export default {
        name: "MenuBar",
        data() {
            return {
            }
        }
    }
</script>

<style scoped>
    #menubar {
        margin-top: 5px;
        height: 100px;
    }

    #menubarLeft {
        text-align: left;
        margin-left: 20px;
        width: 500px;
        float:left;
        margin-top: 20px;
    }

    #logo {
        height: 50px;
        margin-left: 10px;
    }

    #name {
        height: 50px;
        margin-left: -5px;
    }

    #menubarMiddle {
        text-align: left;
        margin-top: 7px;
        margin-left: 200px;
        width: 500px;
        float:left;
    }

    #menubarRight {
        text-align: right;
        width: 300px;
        float:right;
        margin-top: 20px;
        height: 50px;
        margin-right: 20px;
    }

    .el-select .el-input {
        width: 130px;
    }
    .input-with-select .el-input-group__prepend {
        background-color: #fff;
    }
</style>