<template>
  <div>
    <div class="home"  :style="{backgroundImage: 'url('+require('@/assets/banner_bg.jpg')}">
      <div class="v-container">
        <div class="banner_section">
          <h6>SUMMER COLLECTION</h6>
          <p>
            Fall - Winter <br />
            Collection 2030
          </p>
          <h5>
            A specialist label creating luxury essentials. Ethically crafted
            with an <br />
            unwavering commitment to exceptional quality.
          </h5>
          <div class="banner_button">SHOP NOW</div>
        </div>
      </div>
    </div>

    <br />
    <br />
    <br />

    <div class="v-container mt-15">
      <div class="banner_1">
        <div class="banner_heading">
          <h2>
            Clothing<br />
            Collections 2030
          </h2>
          <div class="Now_button">
            <div class="shop_Now_button">
              <h4>SHOP NOW</h4>
            </div>
          </div>
        </div>
        <img :src="require('@/assets/banner/banner-1.jpg')" />
      </div>
      <div class="banner_2">
        <img :src="require('@/assets/banner/banner-2.jpg')" />
        <div class="banner_heading2">
          <h2>
            Shoes <br />
            Spring 2030
          </h2>
          <div class="Now_button">
            <div class="shop_Now_button">
              <h4>SHOP NOW</h4>
            </div>
          </div>
        </div>
      </div>
      <div class="banner_3">
        <div class="banner_heading">
          <h2>Accessories</h2>
          <div class="Now_button">
            <div class="shop_Now_button">
              <h4>SHOP NOW</h4>
            </div>
          </div>
        </div>
        <img :src="require('@/assets/banner/banner-3.jpg')" />
      </div>
    </div>

    <div class="v-container mt-15">
      <v-row class="justify-space-around">
        <p class="deal_title">Best Seller</p>
        <p class="deal_title">New Arrivals</p>
        <p class="deal_title">Hot Sales 🔥</p>
        <p class="deal_title">Whole Saller</p>
      </v-row>
    </div>
    <br />

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
            <div class="shop_Now_button w-100 
            
            +">
              <h4>Add To Cart</h4>
            </div>
          </div>
            </v-card-item>
          </v-card>
        </div>
      </v-row>
    </div>
    <br /><br /><br /><br />

    <div class="bg-grey-lighten-3 m-15">
      <div class="v-container pt-15" style="height: 400px">
        <div class="d-flex align-center justify-space-around">
          <img :src="require('@/assets/product-sale.png')" />
          <div>
            <h3 class="text-subtitle-2 mb-5" style="color: red">
              DEAL OF THE WEEK
            </h3>
            <h4 class="mb-5 text-h4 font-weight-bold">
              Multi-Pocket Chest <br />
              Bag Black
            </h4>

            <div id="clock" class="mb-5">
              <div class="text-h3 font-weight-bold" style="color: red">
                {{ time }}
              </div>
            </div>
            <div class="Now_button">
              <div class="shop_Now_button w-100 mb-5">
                <h4>SHOP NOW</h4>
              </div>
            </div>
          </div>
        </div>

        <br /><br /><br /><br /><br /><br /><br /><br /><br />
      </div>
    </div>
    <br /><br /><br /><br /><br /><br />
    <div class="v-container">
      <div class="d-flex justify-space-between align-center">
        <div>
          <div class="d-flex">
            <img :src="require('@/assets/instagram/instagram-1.jpg')" />
            <img :src="require('@/assets/instagram/instagram-2.jpg')" />
            <img :src="require('@/assets/instagram/instagram-3.jpg')" />
          </div>
          <div class="d-flex">
            <img :src="require('@/assets/instagram/instagram-4.jpg')" />
            <img :src="require('@/assets/instagram/instagram-5.jpg')" />
            <img :src="require('@/assets/instagram/instagram-6.jpg')" />
          </div>
        </div>

        <div class="ml-15">
          <h5 class="mb-5 text-h4 font-weight-bold">Instagram</h5>
          <p style="color: gray" class="text-subtitle-2 mb-5">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil fuga
            quo, sequi ea, unde recusandae, fugiat suscipit expedita iusto
          </p>
          <h6 class="text-h5 font-weight-bold text-red"># Male_Fashion</h6>
        </div>
      </div>
    </div>

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
      ],
      time: "",
      date: "",
      week: ["SUN", "MON", "TUE", "WED", "THU", "FRI", "SAT"],
    };
  },

  mounted() {
    this.updateTime();
    setInterval(this.updateTime, 1000);
  },
  methods: {
    updateTime() {
      var cd = new Date();
      this.time =
        this.zeroPadding(cd.getHours(), 2) +
        ":" +
        this.zeroPadding(cd.getMinutes(), 2) +
        ":" +
        this.zeroPadding(cd.getSeconds(), 2);
      this.date =
        this.zeroPadding(cd.getFullYear(), 4) +
        "-" +
        this.zeroPadding(cd.getMonth() + 1, 2) +
        "-" +
        this.zeroPadding(cd.getDate(), 2) +
        " " +
        this.week[cd.getDay()];
    },
    zeroPadding(num, digit) {
      var zero = "";
      for (var i = 0; i < digit; i++) {
        zero += "0";
      }
      return (zero + num).slice(-digit);
    },
  },
};
</script>

<style>
.home {
  /* background-image: url("@/assets/banner_bg.jpg"); */
  height: 600px;
}
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
.deal_title {
  font-size: 15px;
  color: white;
  font-weight: 500;
  cursor: pointer;
  background-color: #000000;
  padding: 15px 40px;
  /* border-radius: 5px; */
}
.banner_section p {
  color: #111111;
  font-size: 48px;
  font-weight: 700;
  line-height: 58px;
  margin-bottom: 30px;
}
.banner_section h5 {
  font-size: 16px;
  line-height: 28px;
  margin-bottom: 35px;
  color: gray;
  font-weight: 400;
  margin-bottom: 35px;
}
.banner_button {
  display: inline-block;
  font-size: 13px;
  font-weight: 700;
  text-transform: uppercase;
  padding: 14px 30px;
  color: #ffffff;
  background: #000000;
  letter-spacing: 4px;
}
.banner_1 {
  text-align: end;
  display: flex;
  justify-content: space-between;
  flex-direction: row;
  align-items: center;
}

.banner_heading h2 {
  color: #111111;
  font-weight: 900;
  font-size: 35px;
  line-height: 46px;
  margin-bottom: 10px;
}
.banner_heading2 h2 {
  color: #111111;
  font-weight: 900;
  font-size: 35px;
  line-height: 46px;
  margin-bottom: 10px;
  text-align: end;
}
.banner_2 {
  text-align: start;
  display: flex;
  justify-content: space-between;
  flex-direction: row;
  align-items: center;
}
.banner_3 {
  text-align: end;
  display: flex;
  justify-content: space-between;
  flex-direction: row;
  align-items: center;
}
.Now_button {
  display: flex;
  justify-content: end;
  width: 100%;
}
.shop_Now_button {
  border: 2px solid black;
  /* width: 50%; */
  padding: 5px 40px;
  text-align: center;
  cursor: pointer;
  margin-top: 10px;
}
.shop_Now_button:hover {
  border: 2px solid rgba(251, 86, 3, 0.894);
  color: rgba(251, 86, 3, 0.894);
}
</style>
