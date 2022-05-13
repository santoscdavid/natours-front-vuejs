<template>
    <div>
        <About />
        <Features />
    </div>
</template>

<script>
import About from './About.vue';
import Features from './Features.vue';
export default {
    name: 'Main',
    components: { About, Features }
};
</script>

<style></style>
