<template>
  <div class="products">
    <div 
      class="product" 
      v-bind:class="{not_exist: !good.exist }"
      v-for="good in goods"
    >
      <img :src="good.src" alt="" class="product__image">
      <div class="product__info">
        <a href="/" class="product__title">{{good.title}}</a>
        <div v-if="good.exist" class="product__footer">
          <div class="product__price">
            <span v-show="good.old_price" class="product__old-price">{{good.old_price}} $</span>
            <span v-show="good.price" class="product__current-price">{{good.price}} $</span>
          </div>
          <button class="btn product__buy">Купить</button>
        </div>
        <span v-else class="product__not-exist">Продана на аукционе</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    goods: [
      {
        src: require('../assets/img/painting-1.png'), 
        title: '«Рождение Венеры» Сандро Боттичелли', 
        old_price: 2000000, 
        price: 1000000,
        exist: true
      },
      {
        src: require('../assets/img/painting-2.png'), 
        title: '«Тайная вечеря»  Леонардо да Винчи', 
        price: 3000000,
        exist: true
      },
      {
        src: require('../assets/img/painting-3.png'), 
        title: '«Сотворение Адама» Микеланджело', 
        old_price: 6000000, 
        price: 5000000,
        exist: true
      },
      {
        src: require('../assets/img/painting-4.png'), 
        title: '«Урок анатомии»  Рембрандт',
        exist: false,
        info: null
      },
    ]
  }),
  // mounted() {
  //   axios
  //     .get('https://jsonplaceholder.typicode.com/posts/1').then(response => (this.info = response));
  // }
}
</script>