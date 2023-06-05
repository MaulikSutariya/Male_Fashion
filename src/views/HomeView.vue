<template>
  <div>
    <div class="home">
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

    <!-- <div class="v-container mt-15">
      <v-row class="justify-space-around">
        <p class="deal_title">Best Seller</p>
        <p class="deal_title">New Arrivals</p>
        <p class="deal_title">Hot Sales 🔥</p>
        <p class="deal_title">Whole Saller </p>
      </v-row>
    </div> -->

    <br /><br /><br /><br /><br /><br /><br /><br /><br />
  </div>
</template>

<script>
export default {};
</script>

<style>
.home {
  background-image: url("@/assets/banner_bg.jpg");
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
  padding: 30px 40px;
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
  padding: 5px 20px;
  text-align: center;
  cursor: pointer;
  margin-top: 10px;
}
.shop_Now_button:hover {
  border: 2px solid rgba(251, 86, 3, 0.894);
  color: rgba(251, 86, 3, 0.894);
}
</style>
