<template>
    <div>
        <About />
        <Features />
        <Tours />
    </div>
</template>

<script>
import About from './About.vue';
import Features from './Features.vue';
import Tours from './Tours.vue';
export default {
    name: 'Main',
    components: { About, Features, Tours }
};
</script>

<style></style>
