<template>
  <header class="header">
    <div class="container">
      <div class="header__content">
        <div class="menu-block">
          <router-link to="/" class="logo">
            <img src="@/assets/img/logo.png" alt="">
          </router-link>
          <Menu />
        </div>
        <form class="search header__search">
          <input type="text" class="search__input" placeholder="Поиск по названию картины">
          <button class="btn search__button">Найти</button>
        </form>
      </div>
    </div>
  </header>
</template>

<script>
import Menu from '@/components/Menu'

export default {
  components: {
    Menu
  }
}
</script>