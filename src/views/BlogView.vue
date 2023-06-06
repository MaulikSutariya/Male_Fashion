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
      <v-row class="flex-wrap justify-space-around">
        <div class="bg-white d-flex flex-wrap">
          <div v-for="item in items" :key="item.index" class="mb-15 mr-10">
            <div class="">
              <!-- <img :src="require('@/assets/blog/blog-1.jpg')" /> -->
              <img :src="item.img" />
            </div>
            <div class="">
              <span>
                <img :src="require('@/assets/calendar.png')" /> &nbsp;
                {{ item.date }}</span
              >
              <h5 class="mt-2">{{ item.title }}</h5>
              <div
                class="bg-black d-flex align-center justify-space-between"
                style="padding: 10px 20px; margin-top: 15px"
              >
                <h5 class="text-subtitle-1 font-weight-bold">Read More</h5>
                <svg
                  style="cursor: pointer"
                  xmlns="http://www.w3.org/2000/svg"
                  width="19"
                  height="19"
                  fill="currentColor"
                  class="bi bi-arrow-right-circle-fill"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M8 0a8 8 0 1 1 0 16A8 8 0 0 1 8 0zM4.5 7.5a.5.5 0 0 0 0 1h5.793l-2.147 2.146a.5.5 0 0 0 .708.708l3-3a.5.5 0 0 0 0-.708l-3-3a.5.5 0 1 0-.708.708L10.293 7.5H4.5z"
                  />
                </svg>
              </div>
            </div>
          </div>
        </div>
      </v-row>
    </div>
    <!-- blog end -->
    <br />
    <br />
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          date: "16 February 2020",
          title: "What Curling Irons Are The Best Ones",
          img: require("@/assets/blog/blog-1.jpg"),
        },
        {
          date: "21 February 2020",
          title: "Eternity Bands Do Last Forever",
          img: require("@/assets/blog/blog-2.jpg"),
        },
        {
          date: " 28 February 2020",
          title: "The Health Benefits Of Sunglasses",
          img: require("@/assets/blog/blog-3.jpg"),
        },
        {
          date: "16 February 2020",
          title: "Aiming For Higher The Mastopexy",
          img: require("@/assets/blog/blog-4.jpg"),
        },
        {
          date: "21 February 2020",
          title: "Wedding Rings A Gift For A Lifetime",
          img: require("@/assets/blog/blog-5.jpg"),
        },
        {
          date: "28 February 2020",
          title: "The Different Methods Of Hair Removal",
          img: require("@/assets/blog/blog-6.jpg"),
        },
        {
          date: "16 February 2020",
          title: "Hoop Earrings A Style From History",
          img: require("@/assets/blog/blog-7.jpg"),
        },
        {
          date: "21 February 2020",
          title: "Lasik Eye Surgery Are You Ready",
          img: require("@/assets/blog/blog-8.jpg"),
        },
        {
          date: "28 February 2020",
          title: "Lasik Eye Surgery Are You Ready",
          img: require("@/assets/blog/blog-9.jpg"),
        },
      ],
    };
  },
};
</script>

<style></style>
