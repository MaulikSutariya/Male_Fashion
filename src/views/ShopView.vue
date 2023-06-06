<template>
  <div>
    <!-- banner -->
    <div
      :style="{ backgroundImage: 'url(' + require('@/assets/banner_bg2.jpg') }"
    >
      <div class="v-container">
        <div class="banner_section">
          <h6>SUMMER COLLECTION</h6>
          <p>
            Grab Upto 25% Off<br />
            On First Order
          </p>
          <h5>
            A specialist label creating luxury essentials. Ethically crafted
            with an <br />
            unwavering commitment to exceptional quality.
          </h5>
          <div class="banner_button">SHOP NOW</div>
          <br />
          <br />
          <br />
          <br />
          <br />
        </div>
      </div>
    </div>
    <!-- banner end -->

    <!-- product -->
    <div>
      <div class="v-container">
        <v-row class="flex-wrap justify-space-around">
          <div v-for="item in items" :key="item.index">
            <v-card :loading="loading" class="mt-15" max-width="260">
              <template v-slot:loader="{ isActive }">
                <v-progress-linear
                  :active="isActive"
                  color="deep-purple"
                  height="4"
                  indeterminate
                ></v-progress-linear>
              </template>

              <img :src="item.img" />

              <div class="px-2">
                <v-chip-group v-model="selection">
                  <v-chip v-slot="{ isSelected, toggle }"
                    ><svg
                      :color="isSelected ? 'red' : ''"
                      xmlns="http://www.w3.org/2000/svg"
                      width="16"
                      height="16"
                      fill="currentColor"
                      class="bi bi-star"
                      viewBox="0 0 16 16"
                      @click="toggle"
                    >
                      <path
                        d="M2.866 14.85c-.078.444.36.791.746.593l4.39-2.256 4.389 2.256c.386.198.824-.149.746-.592l-.83-4.73 3.522-3.356c.33-.314.16-.888-.282-.95l-4.898-.696L8.465.792a.513.513 0 0 0-.927 0L5.354 5.12l-4.898.696c-.441.062-.612.636-.283.95l3.523 3.356-.83 4.73zm4.905-2.767-3.686 1.894.694-3.957a.565.565 0 0 0-.163-.505L1.71 6.745l4.052-.576a.525.525 0 0 0 .393-.288L8 2.223l1.847 3.658a.525.525 0 0 0 .393.288l4.052.575-2.906 2.77a.565.565 0 0 0-.163.506l.694 3.957-3.686-1.894a.503.503 0 0 0-.461 0z"
                      /></svg
                  ></v-chip>

                  <v-chip
                    ><svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="16"
                      height="16"
                      fill="currentColor"
                      class="bi bi-star"
                      viewBox="0 0 16 16"
                    >
                      <path
                        d="M2.866 14.85c-.078.444.36.791.746.593l4.39-2.256 4.389 2.256c.386.198.824-.149.746-.592l-.83-4.73 3.522-3.356c.33-.314.16-.888-.282-.95l-4.898-.696L8.465.792a.513.513 0 0 0-.927 0L5.354 5.12l-4.898.696c-.441.062-.612.636-.283.95l3.523 3.356-.83 4.73zm4.905-2.767-3.686 1.894.694-3.957a.565.565 0 0 0-.163-.505L1.71 6.745l4.052-.576a.525.525 0 0 0 .393-.288L8 2.223l1.847 3.658a.525.525 0 0 0 .393.288l4.052.575-2.906 2.77a.565.565 0 0 0-.163.506l.694 3.957-3.686-1.894a.503.503 0 0 0-.461 0z"
                      /></svg
                  ></v-chip>

                  <v-chip
                    ><svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="16"
                      height="16"
                      fill="currentColor"
                      class="bi bi-star"
                      viewBox="0 0 16 16"
                    >
                      <path
                        d="M2.866 14.85c-.078.444.36.791.746.593l4.39-2.256 4.389 2.256c.386.198.824-.149.746-.592l-.83-4.73 3.522-3.356c.33-.314.16-.888-.282-.95l-4.898-.696L8.465.792a.513.513 0 0 0-.927 0L5.354 5.12l-4.898.696c-.441.062-.612.636-.283.95l3.523 3.356-.83 4.73zm4.905-2.767-3.686 1.894.694-3.957a.565.565 0 0 0-.163-.505L1.71 6.745l4.052-.576a.525.525 0 0 0 .393-.288L8 2.223l1.847 3.658a.525.525 0 0 0 .393.288l4.052.575-2.906 2.77a.565.565 0 0 0-.163.506l.694 3.957-3.686-1.894a.503.503 0 0 0-.461 0z"
                      /></svg
                  ></v-chip>

                  <v-chip
                    ><svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="16"
                      height="16"
                      fill="currentColor"
                      class="bi bi-star"
                      viewBox="0 0 16 16"
                    >
                      <path
                        d="M2.866 14.85c-.078.444.36.791.746.593l4.39-2.256 4.389 2.256c.386.198.824-.149.746-.592l-.83-4.73 3.522-3.356c.33-.314.16-.888-.282-.95l-4.898-.696L8.465.792a.513.513 0 0 0-.927 0L5.354 5.12l-4.898.696c-.441.062-.612.636-.283.95l3.523 3.356-.83 4.73zm4.905-2.767-3.686 1.894.694-3.957a.565.565 0 0 0-.163-.505L1.71 6.745l4.052-.576a.525.525 0 0 0 .393-.288L8 2.223l1.847 3.658a.525.525 0 0 0 .393.288l4.052.575-2.906 2.77a.565.565 0 0 0-.163.506l.694 3.957-3.686-1.894a.503.503 0 0 0-.461 0z"
                      /></svg
                  ></v-chip>
                  <v-chip
                    ><svg
                      xmlns="http://www.w3.org/2000/svg"
                      width="16"
                      height="16"
                      fill="currentColor"
                      class="bi bi-star"
                      viewBox="0 0 16 16"
                    >
                      <path
                        d="M2.866 14.85c-.078.444.36.791.746.593l4.39-2.256 4.389 2.256c.386.198.824-.149.746-.592l-.83-4.73 3.522-3.356c.33-.314.16-.888-.282-.95l-4.898-.696L8.465.792a.513.513 0 0 0-.927 0L5.354 5.12l-4.898.696c-.441.062-.612.636-.283.95l3.523 3.356-.83 4.73zm4.905-2.767-3.686 1.894.694-3.957a.565.565 0 0 0-.163-.505L1.71 6.745l4.052-.576a.525.525 0 0 0 .393-.288L8 2.223l1.847 3.658a.525.525 0 0 0 .393.288l4.052.575-2.906 2.77a.565.565 0 0 0-.163.506l.694 3.957-3.686-1.894a.503.503 0 0 0-.461 0z"
                      /></svg
                  ></v-chip>
                </v-chip-group>
              </div>

              <v-card-item>
                <v-card-title class=""></v-card-title>
                <v-card-subtitle>
                  <span class="me-1">{{ item.product }}</span>
                </v-card-subtitle>
                <v-card-title class="font-weight-bold text-subtitle-1"
                  >₹ {{ item.price }}</v-card-title
                >
                <div class="Now_button">
                  <div class="shop_Now_button w-100 +">
                    
                    <router-link  style="text-decoration: none" to="/cart"><h4 class="text-black">Add To Cart</h4></router-link>
                  </div>
                </div>
              </v-card-item>
            </v-card>
          </div>
        </v-row>
      </div>
    </div>
    <!-- product end -->
        <br /><br /><br /><br />
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          product: "Piqué Biker Jacket",
          price: "1500",
          img: require("@/assets/product/product-1.jpg"),
        },
        {
          product: "Multi-pocket Chest Bag",
          price: "1000",
          img: require("@/assets/product/product-2.jpg"),
        },
        {
          product: "Diagonal Textured Cap",
          price: "500",
          img: require("@/assets/product/product-3.jpg"),
        },
        {
          product: "Lether Backpack",
          price: "1800",
          img: require("@/assets/product/product-4.jpg"),
        },
        {
          product: "Ankle Boots",
          price: "1400",
          img: require("@/assets/product/product-5.jpg"),
        },
        {
          product: "T-shirt Contrast Pocket",
          price: "1100",
          img: require("@/assets/product/product-6.jpg"),
        },
        {
          product: "Basic Flowing Scarf",
          price: "1150",
          img: require("@/assets/product/product-7.jpg"),
        },
        {
          product: "Piqué Biker Jacket",
          price: "1599",
          img: require("@/assets/product/product-8.jpg"),
        },
        {
          product: "T-shirt Contrast Pocket",
          price: "1100",
          img: require("@/assets/product/product-6.jpg"),
        },
        {
          product: "Basic Flowing Scarf",
          price: "1150",
          img: require("@/assets/product/product-7.jpg"),
        },
        {
          product: "Piqué Biker Jacket",
          price: "1599",
          img: require("@/assets/product/product-8.jpg"),
        },
        {
          product: "Piqué Biker Jacket",
          price: "1599",
          img: require("@/assets/product/product-8.jpg"),
        },
      ],
    };
  },
};
</script>

<style>
.banner_section {
  padding-top: 110px;
}
.banner_section h6 {
  color: #e53637;
  letter-spacing: 2px;
  font-size: 14px;
  font-weight: 700;
  margin-bottom: 28px;
}
</style>
