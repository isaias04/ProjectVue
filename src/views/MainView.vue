<template>
    <div class="container">
        <Isa></Isa>
        <div class="content">
            <router-view></router-view>
        </div>

    </div>
</template>
<script setup>
import Isa from '@/components/Isa.vue';
</script>
<style scoped>
.container {
    display: flex;
}
.content {
    flex: 1;
    padding: 20px;
}
</style>