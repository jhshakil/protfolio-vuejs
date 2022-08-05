<template>
    <div class="px-8 py-3 flex justify-between items-center sticky top-0 bg-gray-100">
        <router-link to="/"><h2 class="text-xl font-bold">jhshakil</h2></router-link>
        <div>
            <ul class="flex gap-3 text-sm font-bold">
                <li>
                <router-link to="/">Home</router-link>
                </li>
                <li>
                <router-link to="/projects">Project</router-link>
                </li>
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