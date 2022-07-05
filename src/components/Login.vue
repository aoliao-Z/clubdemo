<template>
    <div class="login center">
        <div class="shadow">
            <p class="center title">登录</p>
            <div class="center">
                <el-form class="login-form" :model="form" size="large">
                    <el-form-item>
                        <el-input v-model="form.username" placeholder="输入账号" />
                    </el-form-item>
                    <el-form-item>
                        <el-input v-model="form.password" placeholder="输入密码" />
                    </el-form-item>
                    <div class="center">
                        <el-form-item>
                            <el-radio-group v-model="form.method" size="small">
                                <el-radio-button label="get" />
                                <el-radio-button label="post" />
                            </el-radio-group>
                        </el-form-item>
                    </div>
                </el-form>
            </div>
            <div class="btn center">
                <el-button type="primary" @click="onSubmit">Query</el-button>
            </div>
        </div>
    </div>
</template>

<script lang="ts" setup>
import { reactive } from "vue"

const form = reactive({
    username: "",
    password: "",
    method: "post",
})

const onSubmit = () => {
    console.log("submit!")
}
</script>

<style>
.login {
    padding: 50px;
}
.login-form {
    width: 400px;
    padding: 20px 20px;
}
.btn {
    margin-bottom: 20px;
}

.title {
    padding: 10px 0;
}
</style>
