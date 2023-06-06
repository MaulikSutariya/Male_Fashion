<template>
  <div>
    <!-- banner -->
    <div
      :style="{ backgroundImage: 'url(' + require('@/assets/banner_bg.jpg') }"
    >
      <div class="v-container">
        <div class="banner_section">
          <h6>SUMMER COLLECTION</h6>
          <p>Shoping Cart</p>
          <h5>
            Enjoy Shoping and
            <br />
            Get Everything You Want
          </h5>
          <div class="banner_button">SHOP NOW</div>
          <br />
          <br />
          <br />
          <br />
          <br />
          <br />
        </div>
      </div>
    </div>
    <!-- banner end -->

    <!-- cart -->
    <br />
    <br />
    <br />
    <br />

    <div class="v-container">
      <div class="d-flex justify-space-between">
        <div class="">
          <div class="table-responsive shopping-summery">
            <table class="table table-wishlist">
              <thead>
                <tr class="align-center">
                  <th scope="col" class="border-b pb-3" colspan="3">Product</th>
                  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
                  <th scope="col" class="pr-5 border-b pb-3">Unit Price</th>
                  <th scope="col" class="pr-5 border-b pb-3">Quantity</th>
                  <th scope="col" class="pr-5 border-b pb-3">Subtotal</th>
                  <th scope="col" class="pr-5 border-b pb-3">Remove</th>
                </tr>
              </thead>
              &nbsp;
              <tbody>
                <tr class="pt-30">
                  <td class="image product-thumbnail pt-40">
                    <img
                      :src="require('@/assets/product-sale.png')"
                      style="height: 70px; margin-right: 15px"
                    />
                  </td>
                  <td class="product-des product-name">
                    <h6 class="text-subtitle-1 font-weight-bold">
                      Multi-Pocket Chest Bag Black
                    </h6>
                  </td>
                  <td class="product-des product-name"></td>
                  <td class="product-des product-name"></td>
                  <td class="price" data-title="Price">
                    <h4 class="text-body text-center">$2.51</h4>
                  </td>
                  <td class="text-center detail-info" data-title="Stock">
                    <div class="detail-extralink">
                      <div class="detail-qty">
                        <span class="qty-val">1</span>
                      </div>
                    </div>
                  </td>
                  <td class="price" data-title="Price">
                    <h4 class="text-brand text-center">$2.51</h4>
                  </td>
                  <td class="price text-center" data-title="Price">
                    <svg
                      style="color: red"
                      xmlns="http://www.w3.org/2000/svg"
                      width="16"
                      height="16"
                      fill="currentColor"
                      class="bi bi-trash3-fill"
                      viewBox="0 0 16 16"
                    >
                      <path
                        d="M11 1.5v1h3.5a.5.5 0 0 1 0 1h-.538l-.853 10.66A2 2 0 0 1 11.115 16h-6.23a2 2 0 0 1-1.994-1.84L2.038 3.5H1.5a.5.5 0 0 1 0-1H5v-1A1.5 1.5 0 0 1 6.5 0h3A1.5 1.5 0 0 1 11 1.5Zm-5 0v1h4v-1a.5.5 0 0 0-.5-.5h-3a.5.5 0 0 0-.5.5ZM4.5 5.029l.5 8.5a.5.5 0 1 0 .998-.06l-.5-8.5a.5.5 0 1 0-.998.06Zm6.53-.528a.5.5 0 0 0-.528.47l-.5 8.5a.5.5 0 0 0 .998.058l.5-8.5a.5.5 0 0 0-.47-.528ZM8 4.5a.5.5 0 0 0-.5.5v8.5a.5.5 0 0 0 1 0V5a.5.5 0 0 0-.5-.5Z"
                      />
                    </svg>
                  </td>
                </tr>

                <br />
                <tr>
                  <td class="image product-thumbnail">
                    <img
                      :src="require('@/assets/product-sale.png')"
                      style="height: 70px"
                    />
                  </td>
                  <td class="product-des product-name">
                    <h6 class="text-subtitle-1 font-weight-bold">
                      Multi-Pocket Chest Bag Black
                    </h6>
                  </td>
                  <td class="product-des product-name"></td>
                  <td class="product-des product-name"></td>
                  <td class="price" data-title="Price">
                    <h4 class="text-body text-center">$3.2</h4>
                  </td>
                  <td class="text-center detail-info" data-title="Stock">
                    <div class="detail-extralink">
                      <div class="detail-qty">
                        <span class="qty-val">1</span>
                      </div>
                    </div>
                  </td>
                  <td class="price" data-title="Price">
                    <h4 class="text-brand text-center">$3.2</h4>
                  </td>
                  <td class="price text-center" data-title="Price">
                    <svg
                      style="color: red"
                      xmlns="http://www.w3.org/2000/svg"
                      width="16"
                      height="16"
                      fill="currentColor"
                      class="bi bi-trash3-fill"
                      viewBox="0 0 16 16"
                    >
                      <path
                        d="M11 1.5v1h3.5a.5.5 0 0 1 0 1h-.538l-.853 10.66A2 2 0 0 1 11.115 16h-6.23a2 2 0 0 1-1.994-1.84L2.038 3.5H1.5a.5.5 0 0 1 0-1H5v-1A1.5 1.5 0 0 1 6.5 0h3A1.5 1.5 0 0 1 11 1.5Zm-5 0v1h4v-1a.5.5 0 0 0-.5-.5h-3a.5.5 0 0 0-.5.5ZM4.5 5.029l.5 8.5a.5.5 0 1 0 .998-.06l-.5-8.5a.5.5 0 1 0-.998.06Zm6.53-.528a.5.5 0 0 0-.528.47l-.5 8.5a.5.5 0 0 0 .998.058l.5-8.5a.5.5 0 0 0-.47-.528ZM8 4.5a.5.5 0 0 0-.5.5v8.5a.5.5 0 0 0 1 0V5a.5.5 0 0 0-.5-.5Z"
                      />
                    </svg>
                  </td>
                </tr>
                <br />
                <tr>
                  <td class="image product-thumbnail">
                    <img
                      :src="require('@/assets/product-sale.png')"
                      style="height: 70px"
                    />
                  </td>
                  <td class="product-des product-name">
                    <h6 class="text-subtitle-1 font-weight-bold">
                      Multi-Pocket Chest Bag Black
                    </h6>
                  </td>
                  <td class="product-des product-name"></td>
                  <td class="product-des product-name"></td>
                  <td class="price" data-title="Price">
                    <h4 class="text-body text-center">$2.43</h4>
                  </td>
                  <td class="text-center detail-info" data-title="Stock">
                    <div class="detail-extralink">
                      <div class="detail-qty">
                        <span class="qty-val">1</span>
                      </div>
                    </div>
                  </td>
                  <td class="price" data-title="Price">
                    <h4 class="text-brand text-center">$2.43</h4>
                  </td>
                  <td class="price text-center" data-title="Price">
                    <svg
                      style="color: red"
                      xmlns="http://www.w3.org/2000/svg"
                      width="16"
                      height="16"
                      fill="currentColor"
                      class="bi bi-trash3-fill"
                      viewBox="0 0 16 16"
                    >
                      <path
                        d="M11 1.5v1h3.5a.5.5 0 0 1 0 1h-.538l-.853 10.66A2 2 0 0 1 11.115 16h-6.23a2 2 0 0 1-1.994-1.84L2.038 3.5H1.5a.5.5 0 0 1 0-1H5v-1A1.5 1.5 0 0 1 6.5 0h3A1.5 1.5 0 0 1 11 1.5Zm-5 0v1h4v-1a.5.5 0 0 0-.5-.5h-3a.5.5 0 0 0-.5.5ZM4.5 5.029l.5 8.5a.5.5 0 1 0 .998-.06l-.5-8.5a.5.5 0 1 0-.998.06Zm6.53-.528a.5.5 0 0 0-.528.47l-.5 8.5a.5.5 0 0 0 .998.058l.5-8.5a.5.5 0 0 0-.47-.528ZM8 4.5a.5.5 0 0 0-.5.5v8.5a.5.5 0 0 0 1 0V5a.5.5 0 0 0-.5-.5Z"
                      />
                    </svg>
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
          <br />

          <hr />
          <br />
          <br />

          <div class="d-flex justify-space-between">
            <div class="bg-black pt-3 pr-5 pl-5" style="height: 50px">
              <router-link style="text-decoration: none" to="/shop"
                ><h4 class="text-white text-subtitle-1">
                  Continue Shopping
                </h4></router-link
              >
            </div>
            <div class="bg-black pt-3 pr-5 pl-5" style="height: 50px">
              Update Cart
            </div>
          </div>
        </div>
        <div class="p-5">
          <div class="border" style="width: 330px; text-align: center">
            <div
              class="table-responsive"
              style="padding: 30px; text-align: center"
            >
              <div class="d-flex align-center justify-space-between">
                <h6 class="text-h6 font-weight-bold">Subtotal</h6>

                <h4 class="text-brand text-end">$12.31</h4>
              </div>

              <div class="divider-2 mt-10 mb-10"></div>

              <div class="d-flex align-center justify-space-between">
                <div>
                  <h6 class="text-subtitle-1 text-start">Shipping</h6>

                  <h6 class="text-subtitle-1">Estimate for</h6>
                </div>

                <div>
                  <h5 class="text-heading text-end">Free</h5>

                  <h5 class="text-heading text-end">United Kingdom</h5>
                </div>
              </div>

              <div class="divider-2 mt-10 mb-10"></div>

              <div class="d-flex align-center justify-space-between">
                <h6 class="text-subtitle-1 font-weight-bold">Total</h6>

                <h4 class="text-brand text-end">$12.31</h4>
              </div>
            </div>
            <div class="bg-black pt-3 pr-5 pl-5" style="height: 50px">
              Proceed To CheckOut
            </div>
          </div>
        </div>
      </div>
    </div>

    <br />
    <br />
    <br />
    <br />

    <!-- cart end -->
  </div>
</template>

<script>
export default {};
</script>

<style></style>
