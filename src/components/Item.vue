<template>
    <div class="item" id="item">
        <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
            <el-menu-item index="1">Clothes</el-menu-item>
            <el-submenu index="2">
                <template slot="title">Toys</template>
                <el-menu-item index="2-1">选项1</el-menu-item>
                <el-menu-item index="2-2">选项2</el-menu-item>
                <el-menu-item index="2-3">选项3</el-menu-item>
                <el-submenu index="2-4">
                    <template slot="title">选项4</template>
                    <el-menu-item index="2-4-1">选项1</el-menu-item>
                    <el-menu-item index="2-4-2">选项2</el-menu-item>
                    <el-menu-item index="2-4-3">选项3</el-menu-item>
                </el-submenu>
            </el-submenu>
            <el-menu-item index="4">Foods</el-menu-item>
        </el-menu>
        <div class="line"></div>


        <el-row :gutter="20" v-for="item in listData" :key="item">
            <el-col :span="6" v-for="(o, index) in item" :key="o" >
                <el-card :body-style="{ padding: '0px' }">
                    <a href="#"><img src="../assets/baby_clothes.png" class="image"></a>
                    <div style="padding: 14px;">
                        <span>baby clothes</span>
                        <div>
                            <span>77.45$</span>
                        </div>
                    </div>
                </el-card>
            </el-col>
        </el-row>
    </div>
</template>

<script>
    export default {
        name: "Item",
        data() {
            return {
              listData: {"line1": ["a", "b", "C", "d"], "line2": ["a", "b", "c", ]}
            };
        },
        methods: {
            handleSelect() {
                this.$notify({
                    title: '成功',
                    message: '这是一条成功的提示消息',
                    type: 'success'
                });
            }
        }
    }
</script>

<style scoped>
    .item {
        margin-left: 100px;
        margin-right: 100px;
        font-family: 'CGB';
    }

    .el-row {
        margin-bottom: 20px;
    }
    :last-child {
         margin-bottom: 0;
     }
    .el-col {
        border-radius: 4px;
    }
    .bg-purple-dark {
        background: #99a9bf;
    }
    .bg-purple {
        background: #d3dce6;
    }
    .bg-purple-light {
        background: #e5e9f2;
    }
    .grid-content {
        border-radius: 4px;
        min-height: 400px;
    }
    .row-bg {
        padding: 10px 0;
        background-color: #f9fafc;
    }

    .bottom {
        margin-top: 13px;
        line-height: 12px;
    }

    .button {
        padding: 0;
        float: right;
    }

    .image {
        width: 70%;
    }

    .clearfix:before,
    .clearfix:after {
        display: table;
        content: "";
    }

    .clearfix:after {
        clear: both
    }
</style>