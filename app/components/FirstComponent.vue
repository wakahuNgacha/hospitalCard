<template>
    <div class="hero">
        <img src="~/assets/images/p6.svg" alt="">
        <div class="content">
            <h1>Get All your Health records All In One Place</h1>

            <nuxt-link to="/home">
                <button>Get Started</button>                
            </nuxt-link>

        </div>
    </div>
</template>
<script setup>
</script>

<style scoped>
.hero {
    width: 100%;
    height: 90vh;
    /* background-color: lightgray; */
    border-radius: 20px;
}
.hero img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 20px;
    border: 1px solid var(--boder);
}
.content {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
    text-align: center;
}
h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
}
button{
    background-color: var(--text-dark);
}
</style>
