<script lang="ts" setup>
import { ref } from "vue"

const welcomeText = ref("对web感兴趣吗？加入我们!")
</script>

<template>
    <div class="welcome">{{ welcomeText }}</div>
</template>

<style>
.welcome {
    text-align: center;
    padding: 20px 20px;
}
</style>
