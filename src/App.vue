<template>
    <nav-bar />
    <wel-come />
    <login />
    <wrap title="大致步骤">
        <steps />
    </wrap>

    <wrap title="日期查看">
        <calendar />
    </wrap>
    <Foot />
</template>

<script lang="ts" setup>
import NavBar from "./components/NavBar.vue"
import WelCome from "./components/WelCome.vue"
import Login from "./components/Login.vue"
import Wrap from "./components/Wrap.vue"
import Steps from "./components/Steps.vue"
import Calendar from "./components/Calendar.vue"
import Foot from "./components/Foot.vue"
</script>

<style>
* {
    margin: 0;
}
</style>
