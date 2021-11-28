<template>
  <footer class='bg-purple-400'>
    <div class="container flex justify-between items-center p-7 text-white">
      <div v-html="foot.footer"></div>
      <ul>
        <li><NuxtLink to='#'>About</NuxtLink></li>
        <li><NuxtLink to='#'>Contact</NuxtLink></li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  props: ['foot']
}
</script>
