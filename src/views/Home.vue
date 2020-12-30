<template>
  <div class="container">
    <h1 class="page__title">Картины эпохи Возрождения</h1>
    <ProductList />
  </div>
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
