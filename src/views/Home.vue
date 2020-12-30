<template>
  <main class="page">
    <div class="container">
      <h1 class="page__title">Картины эпохи Возрождения</h1>
      <ProductList />
    </div>
  </main>
</template>

<script>
import ProductList from '@/components/ProductList'

export default {
  name: 'Home',
  components: {
    ProductList
  }
}
</script>
