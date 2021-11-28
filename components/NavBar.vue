<template>
    <nav class="bg-gradient-to-r from-purple-100 via-purple-300 to-purple-100 p-6">
        <ul class="flex justify-evenly text-2xl font-bold">
            <li><NuxtLink class="hover:text-pink-500" to="/">{{ navItem.link1 }}</NuxtLink></li>
            <li><NuxtLink class="hover:text-pink-500" to="#">{{ navItem.link2 }}</NuxtLink></li>
            <li><NuxtLink class="hover:text-pink-500" to="/gallery">{{ navItem.link3 }}</NuxtLink></li>
            <li><NuxtLink class="hover:text-pink-500" to="#">{{ navItem.link4 }}</NuxtLink></li>
        </ul>
    </nav>
</template>

<script>
export default {
  props: ['navItem']
}
</script>
