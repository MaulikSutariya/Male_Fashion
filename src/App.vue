<template>
  <div class="home">
    <NavbarView />
  </div>
</template>

<script>
// @ is an alias to /src
import NavbarView from '@/views/NavbarView.vue'

export default {
  name: 'HomeView',
  components: {
    NavbarView
  }
}
</script>

