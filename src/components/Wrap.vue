<script lang="ts" setup>
import { defineProps } from "vue"
type WrapProps = {
    title: string
}
const props = defineProps<WrapProps>()
</script>

<template>
    <div>
        <el-divider content-position="left">{{ props.title }}</el-divider>
        <div class="center">
            <div class="shadow child">
                <slot />
            </div>
        </div>
    </div>
</template>
<style>
.child {
    padding: 10px;
}
</style>
