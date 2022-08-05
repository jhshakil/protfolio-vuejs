<template>
    <div class="my-12 lg:my-16 mx-2 lg:mx-16">
        <h2 class="text-2xl lg:text-4xl font-bold text-center">My Project</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-12 mt-8 lg:mt-16 items-center">
            <img src="../assets/project1/project1.jpg" class="rounded-lg" alt="Project 1">
            <div>
                <h3 class="text-xl lg:text-2xl font-bold text-centertext-2xl font-bold text-center my-4">Manufacture Website</h3>
                <p class="text-sm lg:text-lg">This is a manufacturer website. It is a MERN Stack project. This website is controlled by Admin. Admin can add products and manage orders. Here client site code and server site code</p>
                <div class="flex justify-evenly items-center my-4">
                    <div class="mt-4 lg:mt-12 text-sm lg:text-xl">
                        <a target="_blank" class="bg-gray-300 p-2 lg:p-4 rounded-md" href="https://shakils-hardware.web.app/">Live Site</a>
                    </div>
                    <div class="mt-4 lg:mt-12 text-sm lg:text-xl">
                        <a target="_blank" class="bg-gray-300 p-2 lg:p-4 rounded-md" href="https://github.com/jhshakil/shakils-hardware-client">Client Site Code</a>
                    </div>
                    <div class="mt-4 lg:mt-12 text-sm lg:text-xl">
                        <a target="_blank" class="bg-gray-300 p-2 lg:p-4 rounded-md" href="https://github.com/jhshakil/shakils-hardware-server">Server Site Code</a>
                    </div>
                </div>
            </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-12 mt-16 items-center">
            <img src="../assets/project2/project2.jpg" class="rounded-lg order-1 lg:order-2" alt="Project 1">
            <div class="order-2 lg:order-1">
                <h3 class="text-xl lg:text-2xl font-bold text-centertext-2xl font-bold text-center my-4">Warehouse Management Website</h3>
                <p class="text-sm lg:text-lg">This is a Warehouse Management Website. It is a MERN Stack project. Add product, Add Quantity and Delete Product are the main feature in this website. Here client site code and server site code</p>
                <div class="flex justify-evenly items-center my-4">
                    <div class="mt-4 lg:mt-12 text-sm lg:text-xl">
                        <a target="_blank" class="bg-gray-300 p-2 lg:p-4 rounded-md" href="https://car-dealer-af8e9.web.app/">Live Site</a>
                    </div>
                    <div class="mt-4 lg:mt-12 text-sm lg:text-xl">
                        <a target="_blank" class="bg-gray-300 p-2 lg:p-4 rounded-md" href="https://github.com/jhshakil/warehouse-management-client">Client Site Code</a>
                    </div>
                    <div class="mt-4 lg:mt-12 text-sm lg:text-xl">
                        <a target="_blank" class="bg-gray-300 p-2 lg:p-4 rounded-md" href="https://github.com/jhshakil/warehouse-management-server">Server Site Code</a>
                    </div>
                </div>
            </div>
        </div>
        <div class="flex justify-evenly items-center mt-8 lg:mt-16">
            <div class="text-md lg:text-2xl text-center font-bold">
                <router-link class="bg-orange-200 py-2 lg:py-3 px-3 lg:px-4 rounded-lg" to="/projects">See More ...</router-link>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyProject'
}
</script>