<template>
    <div class="headerHolder">
        <div class="logo">
            <!-- <img src="/logo.png" alt="Hospital Card Logo" /> -->
            <h3>Hospital Card</h3>
        </div>

        <div class="middle">
            <NuxtLink to="/">
                <span>Features</span>
            </NuxtLink>
            <NuxtLink to="/about">
                <span>solutions</span>
            </NuxtLink>
            <NuxtLink to="/contact">
                <span>Documentation</span>
            </NuxtLink>
        </div>

        <div class="callToAction">
            <NuxtLink to="/signup">
                <span>Sign up</span>
            </NuxtLink>
            <button class="getDemo">
                <span>Get demo</span>
            </button>
        </div>        
    </div>


</template>
<script setup>
</script>
<style scoped>
.headerHolder {
    width: 100%;
    height: 80px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    /* background-color: rgb(173, 8, 8); */
}
.middle {
    display: flex;
    gap: 30px;
}
.middle span {
    text-decoration: none;
    cursor: pointer;
}
.callToAction {
    display: flex;
    align-items: center;
    gap: 20px;
}
.getDemo {
    width: auto;
    padding: 10px 5px;
    border: none;
    border-radius: 5px;
    background-color: var(--text-light);
    border: 1px solid var(--boder);
    color: var(--text-light-dark);
    cursor: pointer;
}
</style>
