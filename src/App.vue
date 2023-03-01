<template>
<child :img=images />
</template>

<script>
import child from './components/child.vue'
export default {
  name:'App',
    components: {
        child,
    },
    data() {
        return {
            images: [
                "./src/assets/bree.jpg",
                "./src/assets/el.jpg",
                "./src/assets/klara.jpg",
                "./src/assets/nikita.jpg",

            ],
        };
    },
};
</script>

<style>
</style>