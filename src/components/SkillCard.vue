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

img {
    height: 36px;
}

</style>