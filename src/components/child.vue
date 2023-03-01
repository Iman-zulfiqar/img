<template>
<div class="container">
    <div v-for="i in img"><img :src="i"></div>
</div>
</template>

<script>
export default {
    name: 'child',
    props: {
        img: Array
    },
};
</script>

<style scoped>
.container {
    padding: 10px;
    width: 100vw;
    min-height: 100vh;
    background: #021927;
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    justify-content: space-evenly;
    align-items: center;
    overflow: hidden;
}

.container div {
    height: 350px;
    width: 200px;
}

div img {
    max-width: 300px;
    width: 100%;
    max-height: 600px;
}
</style>
