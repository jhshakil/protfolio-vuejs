<template>
    <div class="bg-gray-100">
        <Navigation></Navigation>
        <AllProject></AllProject>
        <Footer></Footer>
    </div>
</template>

<script>
import Navigation from '../components/Navigation.vue';
import Footer from '../components/Footer.vue';
import AllProject from '@/components/AllProject.vue';

export default {
    name: 'ProjectView',
    components: {
    Navigation,
    Footer,
    AllProject
}
}

</script>