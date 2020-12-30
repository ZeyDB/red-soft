<template>
  <div class="main-layout">
    <Header />
    <main class="page">
      <router-view />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'

export default {
  name: 'MainLayout',
  components: {
    Header, Footer
  }
}
</script>