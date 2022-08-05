<template>
    <div class="bg-gray-100">
        <Navigation></Navigation>
        <div>
            <h2 class="text-4xl lg:text-7xl font-bold text-center flex justify-center items-center h-screen text-red-600">Coming Soon ...</h2>
        </div>
        <Footer></Footer>
    </div>
</template>

<script>
import Navigation from '@/components/Navigation.vue';
import Footer from '@/components/Footer.vue';
export default {
    name: "BlogView",
    components: { 
        Navigation,
        Footer 
        }
}
</script>