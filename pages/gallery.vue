<template>
    <div>
        <NavBar :navItem='galleryAssets'/>
        <HeaderSection :headerItem='galleryAssets'/>
        <GalleryComponent :galleryItem='image' v-for='image in images' :key="image.id" />
        <FooterPart :foot='galleryAssets'/>
    </div>
</template>

<script>
export default {
  data() {
    return {
      galleryAssets: {
        link1: 'Home',
        link2: 'Services',
        link3: 'Gallery',
        link4: 'Contact us',
        footer: '<p>&copy; Raj</p>'
      },
      images: [
        {
          title: 'White Camero',
          credit: 'Peter Broomfield',
          image: 'images/image1.jpg'
        },
        {
          title: 'Black Porsche',
          credit: 'Campbell',
          image: 'images/image2.jpg'
        },
        {
          title: 'Red Porsche',
          credit: 'Dillon Kydd',
          image: 'images/image3.jpg'
        }
      ]
    }
  }
}
</script>
