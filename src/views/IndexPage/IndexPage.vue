<template>
    <div>
        <Header />
        <GridTest />
    </div>
</template>

<script>
import Header from '@/components/Header.vue';
import GridTest from '@/components/Grid-test.vue';
export default {
    name: 'IndexPage',
    components: { Header, GridTest }
};
</script>
