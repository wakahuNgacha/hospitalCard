<template>
    <div class="menuHolder">
        <div v-for="(item, index) in menuItems" :key="index">
        <NuxtLink :to="item.link" class="menuItem">
            <UIcon :name="item.icon" class="size-5" />
            <p>{{ item.text }}</p>
        </NuxtLink>
        </div>
    </div>

</template>
<script setup>
import { link } from '#build/ui';

const props = defineProps({
    menuItems: Object,
});
</script>
<style scoped>
.menuHolder {
    display: flex;
    flex-direction: column;
    align-items: start;
    justify-content: start;
    width: 200px;
    margin-top: 20px;
    padding: 10px;
    /* background-color: blue; */
    border-radius: 20px;
    border: 1px solid var(--boder);
}
.menuItem {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 10px;
    margin-bottom: 10px;
    cursor: pointer;
}
</style>
