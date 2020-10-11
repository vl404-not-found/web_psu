<template>
  <div class="w-100">
    <Header />
    <div>
      <Nuxt />
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/sceleton/Header'
import Footer from '@/components/sceleton/Footer'

export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style scoped>

</style>
