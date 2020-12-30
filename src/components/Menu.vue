<template>
  <ul class="menu header__menu">

    <router-link
      v-for="link in links"
      :key="link.url"
      tag="li"
      class="menu__item"
      to="/"
    >
      <a href="#" class="menu__link">{{ link.title }}</a>
    </router-link>
  </ul>
</template>

<script>
export default {
  data: () => ({
    links: [
      {title: 'Каталог', url: '/catalog'},
      {title: 'Доставка', url: '/delivery'},
      {title: 'Оплата', url: '/pay'},
      {title: 'Контакты', url: '/contacts'},
      {title: 'О галерее', url: '/about'}
    ]
  })
}
</script>