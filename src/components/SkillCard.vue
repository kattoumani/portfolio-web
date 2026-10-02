<template>
    <div class="card">
        <img :src="imageSrc" :alt="name">
        <h3>{{name}}</h3>
    </div>
</template>

<script setup>
defineProps({
    name: String,
    imageSrc: String,
})
</script>

<style scoped>
.card {
    display:flex;
    align-items: center;
    gap: 0.5rem;
}

.section {
    margin: 0 auto;
    width: 1100px;
    height: 125px;
    border: 2px solid #6495ED;
    background-color: #0C0C0D;
}

img {
    height: 36px;
}

</style>