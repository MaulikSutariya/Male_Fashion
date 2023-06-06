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
          <p class="text-white">Contact Us</p>
          <br />
          <br />
        </div>
      </div>
    </div>
    <br/>
    <br/>
    <!-- banner end -->

    <div class="v-container">
      <div class="row d-flex justify-space-between">
        <div class="col-lg-6 col-md-6" style="width:100%">
          <div class="contact__text">
            <div class="section-title">
              
              <h2 class="text-h4 font-weight-bold mb-2">Contact Us</h2>
              <p class="text-subtitle-1 text-grey mb-5">
                As you might expect of a company that began as a high-end<br />
                interiors contractor, we pay strict attention.
              </p>
            </div>
           
                <h4>America</h4>
                <p class="text-subtitle-1 text-grey mb-5">
                  195 E Parker Square Dr, Parker, CO 801 <br />+43 982-314-0958
                </p>
           
                <h4>France</h4>
                <p class="text-subtitle-1 text-grey mb-5">
                  109 Avenue Léon, 63 Clermont-Ferrand <br />+12 345-423-9893
                </p>
           
          </div>
        </div>
        <div class="col-lg-6 col-md-6" style="width:100%">
          <div class="contact__form" style="width:100%">
            <form action="#" style="width:100%">
              <div class="row">
                <div style="width:100%" class="d-flex">
                  <v-text-field  class="mr-5" label="Name"></v-text-field>
                   <v-text-field label="Email"></v-text-field>
                </div>
      
                <div class="col-lg-12">
                  <v-textarea label="Message"></v-textarea>
                  <button class="bg-black d-flex align-center justify-space-between"
                style="padding: 10px 20px; margin-top: 15px" type="submit" >Send Message</button>
                </div>
              </div>
            </form>
          </div>
        </div>
      </div>
      <br />
      <br />
      <br />
      <br />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
