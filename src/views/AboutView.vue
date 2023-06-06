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
          <p class="text-white">About Us</p>
          <br />
          <br />
        </div>
      </div>
    </div>
    <br />
    <br />
    <!-- banner end -->
    <div class="v-container">
      <div class="text-center">
        <img :src="require('@/assets/about/about-us.jpg')" />
      </div>
      <br />
      <div class="d-flex">
        <div class="mr-10 text-justify">
          <h5 class="text-h6 font-weight-bold mb-3">Who We Are ?</h5>
          <p class="text-subtitle-2">
            Contextual advertising programs sometimes have strict policies that
            need to be adhered too. Let’s take Google as an example.
          </p>
        </div>
        <div class="mr-10 text-justify">
          <h5 class="text-h6 font-weight-bold mb-3">Who We Do ?</h5>
          <p class="text-subtitle-2">
            In this digital generation where information can be easily obtained
            within seconds, business cards still have retained their importance.
          </p>
        </div>
        <div class="text-justify">
          <h5 class="text-h6 font-weight-bold mb-3">Why Choose Us ?</h5>
          <p class="text-subtitle-2">
            A two or three storey house is the ideal way to maximise the piece
            of earth on which our home sits, but for older or infirm people.
          </p>
        </div>
      </div>
      <br />

      <br />
      <hr />
    </div>
     <br /> 
   <!--  -->
   <div class="v-container">
    <div class="text-center">
      <h5 class="text-red mb-2">O U R&nbsp;&nbsp;&nbsp; T E A M </h5>
      <h4 class="text-h4 font-weight-bold">Meet Our Team</h4>
    </div>
    <div class="d-flex justify-space-around mt-10">
      <div>
         <img :src="require('@/assets/about/team-1.jpg')" />
         <h5 class="text-h6 font-weight-bold">John Smith</h5>
         <h6 class="text-grey text-subtitle-2">Fashion Design</h6>
      </div>
      <div>
         <img :src="require('@/assets/about/team-2.jpg')" />
         <h5 class="text-h6 font-weight-bold">John Smith</h5>
         <h6 class="text-grey text-subtitle-2">Fashion Design</h6>
      </div>
      <div>
         <img :src="require('@/assets/about/team-3.jpg')" />
         <h5 class="text-h6 font-weight-bold">John Smith</h5>
         <h6 class="text-grey text-subtitle-2">Fashion Design</h6>
      </div>
      <div>
         <img :src="require('@/assets/about/team-4.jpg')" />
         <h5 class="text-h6 font-weight-bold">John Smith</h5>
         <h6 class="text-grey text-subtitle-2">Fashion Design</h6>
      </div>
    </div>
   </div>
    <br />  <br /> 
   <!--  -->

   <div class="v-container ">
    <div class="text-center">
      <h5 class="text-red mb-2">P A R T N E R</h5>
      <h4 class="text-h4 font-weight-bold">Happy Clients</h4>
    </div><br/><br/><br/><br/>
    <div class="d-flex justify-space-around text-center">
        <img :src="require('@/assets/clients/client-1.png')" />
        <img :src="require('@/assets/clients/client-2.png')" />
        <img :src="require('@/assets/clients/client-3.png')" />
        <img :src="require('@/assets/clients/client-4.png')" />
        <img :src="require('@/assets/clients/client-5.png')" />
        <img :src="require('@/assets/clients/client-6.png')" />
        <img :src="require('@/assets/clients/client-7.png')" />
        <img :src="require('@/assets/clients/client-8.png')" />
    </div>
    
   </div>
<br/><br/><br/><br/>
  </div>
</template>
