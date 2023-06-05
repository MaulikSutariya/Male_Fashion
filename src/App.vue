<template>
  <div class="home">
    <NavbarView />
    <FooterView />
  </div>
</template>

<script>
// @ is an alias to /src
import NavbarView from '@/views/NavbarView.vue'
import FooterView from '@/views/FooterView.vue'

export default {
  name: 'HomeView',
  components: {
    NavbarView,
    FooterView
  }
}
</script>

