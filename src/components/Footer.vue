<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__content">
        <div class="menu-block">
          <router-link to="/" class="logo">
            <img src="@/assets/img/logo.png" alt="">
          </router-link>
          <Menu />
        </div>
        <div class="contacts footer__contacts">
          <a href="tel:+74955555555" class="contacts__phone">+7 (495) 555-55-55</a>
          <span class="contacts__adress">г. Москва, ул. Расплетина, 24</span>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import Menu from '@/components/Menu'

export default {
  components: {
    Menu
  }
}
</script>