<template>
    <div class="px-8 py-3 flex justify-between items-center">
        <router-link to="/"><h2 class="text-3xl font-bold">jhshakil</h2></router-link>
        <div>
            <ul class="flex gap-6 text-xl font-bold">
                <li>
                <router-link to="/">Home</router-link>
                </li>
                <!-- <li>
                <router-link to="/project">Project</router-link>
                </li> -->
                <li>
                <router-link to="/blogs">Blogs</router-link>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
  name: 'NaviGation',
}
</script>