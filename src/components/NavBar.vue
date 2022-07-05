<script lang="ts" setup>
import { Search } from "@element-plus/icons-vue"
</script>
<template>
    <div class="nav-bar shadow">
        <h2 class="nav-bar-title">牧码南山试题</h2>
        <div class="nav-bar-icon">
            <el-button :icon="Search" circle />
        </div>
    </div>
</template>

<style>
.nav-bar {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 30px 50px;
}
.nav-bar-title {
}
.nav-bar-icon {
}
</style>
