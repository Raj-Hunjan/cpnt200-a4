<template>
  <article>
    <figure class="flex justify-evenly gap-x-16 gap-y-16 flex-wrap p-16 bg-gradient-to-r from-purple-100 via-purple-200 to-purple-100">
      <div v-html="`<h3>${galleryItem.title}</h3>`"></div>
      <nuxt-img :src="galleryItem.image" sizes="sm:300px md:400px lg:500px" />
      <figcaption v-text="galleryItem.credit" />
    </figure>
  </article>
</template>

<script>
export default {
  props: ['galleryItem']
}
</script>
