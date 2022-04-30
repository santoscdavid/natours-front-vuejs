<template>
    <div>
        <Header />
        <Main />
        <!-- <GridTest /> -->
    </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
// import GridTest from '@/components/Grid-test.vue';
export default {
    name: 'IndexPage',
    components: { Header, Main }
};
</script>
