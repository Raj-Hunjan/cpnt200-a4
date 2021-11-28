<template>
    <div>
        <NavBar :navItem='siteAssets'/>
        <HeroSection :heroItem='siteAssets'/>
        <FooterPart :foot='siteAssets'/>
    </div>
</template>
<script>
export default {
  data() {
    return {
      siteAssets: {
        link1: 'Home',
        link2: 'Services',
        link3: 'Gallery',
        link4: 'Contact us',
        hero: 'Some Website About Things And stuff',
        footer: '<p>&copy; Raj</p>'
      }
    }
  }
}
</script>
