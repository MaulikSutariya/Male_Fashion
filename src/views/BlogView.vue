<template>
  <div>
    <!-- banner -->
    <div
      :style="{
        backgroundImage: 'url(' + require('@/assets/breadcrumb-bg.jpg'),
      }"
    >
      <div class="v-container">
        <div class="text-center text-h2 font-weight-bold">
          <br /><br />
          <p class="text-white">Our Blog</p>
          <br />
          <br />
        </div>
      </div>
    </div>
    <!-- banner end -->
    <br />
    <br />
    <br />
    <!-- blog -->
    <div class="v-container">
      <div class="bg-white">
        <div class="">
          <div class="">
            <img :src="require('@/assets/blog/blog-1.jpg')" />
          </div>
          <div class="">
            <span
              > <img :src="require('@/assets/calendar.png')" /> 16 February 2020</span
            >
            <h5>Aiming For Higher The Mastopexy</h5>
            <a href="#">Read More</a>
          </div>
        </div>
      </div>
    </div>
    <!-- blog end -->
  </div>
</template>

<script>
export default {};
</script>

<style></style>
