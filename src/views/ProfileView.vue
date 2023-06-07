<template>
  <div>
    <br /><br />
    <div class="v-container">
      <div class="d-flex justify-space-around" style="width: 100%">
        <!-- profile -->
        <div style="width: 30%; text-align: center">
          <img
            style="height: 200px; width: 200px; border-radius: 50%"
            :src="require('@/assets/profile.jpg')"
          />
          <br />
          <br />
          <br />
          <div
            class="d-flex align-center bg-grey-lighten-2 mb-5"
            style="padding: 7px 15px; border-radius: 5px"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-person-square"
              viewBox="0 0 16 16"
            >
              <path d="M11 6a3 3 0 1 1-6 0 3 3 0 0 1 6 0z" />
              <path
                d="M2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2zm12 1a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1v-1c0-1-1-4-6-4s-6 3-6 4v1a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1h12z"
              /></svg
            >&nbsp;&nbsp;
            <h5>My Account</h5>
          </div>
          <div
            class="d-flex align-center bg-grey-lighten-2 mb-5"
            style="padding: 7px 15px; border-radius: 5px"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-pencil-square"
              viewBox="0 0 16 16"
            >
              <path
                d="M15.502 1.94a.5.5 0 0 1 0 .706L14.459 3.69l-2-2L13.502.646a.5.5 0 0 1 .707 0l1.293 1.293zm-1.75 2.456-2-2L4.939 9.21a.5.5 0 0 0-.121.196l-.805 2.414a.25.25 0 0 0 .316.316l2.414-.805a.5.5 0 0 0 .196-.12l6.813-6.814z"
              />
              <path
                fill-rule="evenodd"
                d="M1 13.5A1.5 1.5 0 0 0 2.5 15h11a1.5 1.5 0 0 0 1.5-1.5v-6a.5.5 0 0 0-1 0v6a.5.5 0 0 1-.5.5h-11a.5.5 0 0 1-.5-.5v-11a.5.5 0 0 1 .5-.5H9a.5.5 0 0 0 0-1H2.5A1.5 1.5 0 0 0 1 2.5v11z"
              /></svg
            >&nbsp;&nbsp;
            <h5>Chnage Password</h5>
          </div>
          <div
            class="d-flex align-center bg-grey-lighten-2 mb-5"
            style="padding: 7px 15px; border-radius: 5px"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-receipt"
              viewBox="0 0 16 16"
            >
              <path
                d="M1.92.506a.5.5 0 0 1 .434.14L3 1.293l.646-.647a.5.5 0 0 1 .708 0L5 1.293l.646-.647a.5.5 0 0 1 .708 0L7 1.293l.646-.647a.5.5 0 0 1 .708 0L9 1.293l.646-.647a.5.5 0 0 1 .708 0l.646.647.646-.647a.5.5 0 0 1 .708 0l.646.647.646-.647a.5.5 0 0 1 .801.13l.5 1A.5.5 0 0 1 15 2v12a.5.5 0 0 1-.053.224l-.5 1a.5.5 0 0 1-.8.13L13 14.707l-.646.647a.5.5 0 0 1-.708 0L11 14.707l-.646.647a.5.5 0 0 1-.708 0L9 14.707l-.646.647a.5.5 0 0 1-.708 0L7 14.707l-.646.647a.5.5 0 0 1-.708 0L5 14.707l-.646.647a.5.5 0 0 1-.708 0L3 14.707l-.646.647a.5.5 0 0 1-.801-.13l-.5-1A.5.5 0 0 1 1 14V2a.5.5 0 0 1 .053-.224l.5-1a.5.5 0 0 1 .367-.27zm.217 1.338L2 2.118v11.764l.137.274.51-.51a.5.5 0 0 1 .707 0l.646.647.646-.646a.5.5 0 0 1 .708 0l.646.646.646-.646a.5.5 0 0 1 .708 0l.646.646.646-.646a.5.5 0 0 1 .708 0l.646.646.646-.646a.5.5 0 0 1 .708 0l.646.646.646-.646a.5.5 0 0 1 .708 0l.509.509.137-.274V2.118l-.137-.274-.51.51a.5.5 0 0 1-.707 0L12 1.707l-.646.647a.5.5 0 0 1-.708 0L10 1.707l-.646.647a.5.5 0 0 1-.708 0L8 1.707l-.646.647a.5.5 0 0 1-.708 0L6 1.707l-.646.647a.5.5 0 0 1-.708 0L4 1.707l-.646.647a.5.5 0 0 1-.708 0l-.509-.51z"
              />
              <path
                d="M3 4.5a.5.5 0 0 1 .5-.5h6a.5.5 0 1 1 0 1h-6a.5.5 0 0 1-.5-.5zm0 2a.5.5 0 0 1 .5-.5h6a.5.5 0 1 1 0 1h-6a.5.5 0 0 1-.5-.5zm0 2a.5.5 0 0 1 .5-.5h6a.5.5 0 1 1 0 1h-6a.5.5 0 0 1-.5-.5zm0 2a.5.5 0 0 1 .5-.5h6a.5.5 0 0 1 0 1h-6a.5.5 0 0 1-.5-.5zm8-6a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 0 1h-1a.5.5 0 0 1-.5-.5zm0 2a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 0 1h-1a.5.5 0 0 1-.5-.5zm0 2a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 0 1h-1a.5.5 0 0 1-.5-.5zm0 2a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 0 1h-1a.5.5 0 0 1-.5-.5z"
              /></svg
            >&nbsp;&nbsp;
            <h5>Billing Address</h5>
          </div>
          <div
            class="d-flex align-center bg-grey-lighten-2 mb-5"
            style="padding: 7px 15px; border-radius: 5px"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-truck"
              viewBox="0 0 16 16"
            >
              <path
                d="M0 3.5A1.5 1.5 0 0 1 1.5 2h9A1.5 1.5 0 0 1 12 3.5V5h1.02a1.5 1.5 0 0 1 1.17.563l1.481 1.85a1.5 1.5 0 0 1 .329.938V10.5a1.5 1.5 0 0 1-1.5 1.5H14a2 2 0 1 1-4 0H5a2 2 0 1 1-3.998-.085A1.5 1.5 0 0 1 0 10.5v-7zm1.294 7.456A1.999 1.999 0 0 1 4.732 11h5.536a2.01 2.01 0 0 1 .732-.732V3.5a.5.5 0 0 0-.5-.5h-9a.5.5 0 0 0-.5.5v7a.5.5 0 0 0 .294.456zM12 10a2 2 0 0 1 1.732 1h.768a.5.5 0 0 0 .5-.5V8.35a.5.5 0 0 0-.11-.312l-1.48-1.85A.5.5 0 0 0 13.02 6H12v4zm-9 1a1 1 0 1 0 0 2 1 1 0 0 0 0-2zm9 0a1 1 0 1 0 0 2 1 1 0 0 0 0-2z"
              /></svg
            >&nbsp;&nbsp;
            <h5>Shipping Address</h5>
          </div>
          <div
            class="d-flex align-center bg-grey-lighten-2 mb-5"
            style="padding: 7px 15px; border-radius: 5px"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-box2-fill"
              viewBox="0 0 16 16"
            >
              <path
                d="M3.75 0a1 1 0 0 0-.8.4L.1 4.2a.5.5 0 0 0-.1.3V15a1 1 0 0 0 1 1h14a1 1 0 0 0 1-1V4.5a.5.5 0 0 0-.1-.3L13.05.4a1 1 0 0 0-.8-.4h-8.5ZM15 4.667V5H1v-.333L1.5 4h6V1h1v3h6l.5.667Z"
              /></svg
            >&nbsp;&nbsp;
            <h5>My Orders</h5>
          </div>
          <div
            class="d-flex align-center bg-grey-lighten-2 mb-5"
            style="padding: 7px 15px; border-radius: 5px"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-box-arrow-right"
              viewBox="0 0 16 16"
            >
              <path
                fill-rule="evenodd"
                d="M10 12.5a.5.5 0 0 1-.5.5h-8a.5.5 0 0 1-.5-.5v-9a.5.5 0 0 1 .5-.5h8a.5.5 0 0 1 .5.5v2a.5.5 0 0 0 1 0v-2A1.5 1.5 0 0 0 9.5 2h-8A1.5 1.5 0 0 0 0 3.5v9A1.5 1.5 0 0 0 1.5 14h8a1.5 1.5 0 0 0 1.5-1.5v-2a.5.5 0 0 0-1 0v2z"
              />
              <path
                fill-rule="evenodd"
                d="M15.854 8.354a.5.5 0 0 0 0-.708l-3-3a.5.5 0 0 0-.708.708L14.293 7.5H5.5a.5.5 0 0 0 0 1h8.793l-2.147 2.146a.5.5 0 0 0 .708.708l3-3z"
              /></svg
            >&nbsp;&nbsp;
            <h5>Log Out</h5>
          </div>
        </div>
        <!-- profile -->

        <!-- other -->
        <div
          style="
            width: 100%;
            margin-left: 100px;
            padding: 20px;
            border-radius: 10px;
          "
          class="bg-grey-lighten-2"
        >
          <h5
            class="text-h5 font-weight-bold bg-white pl-5 mb-5"
            style="padding: 5px; border-radius: 8px"
          >
            My Account
          </h5>
          <div
            class="bg-white"
            style="padding: 5px; border-radius: 8px; height: 89%"
          >
            <h6 class="text-subtitle-1 mt-3 mb-3 ml-2 font-weight-bold">
              1. Personal Details
            </h6>
            <v-row
              style="padding-top: 10px; padding-left: 20px; padding-right: 20px"
            >
              <v-text-field label="First Name"></v-text-field>&nbsp;&nbsp;&nbsp;
              <v-text-field label="Middle Name"></v-text-field
              >&nbsp;&nbsp;&nbsp;
              <v-text-field label="Last Name"></v-text-field>
            </v-row>
            <v-row style="padding-top5px;padding-left:20px;padding-right:20px">
              <v-text-field label="Email"></v-text-field>&nbsp;&nbsp;&nbsp;
              <v-text-field label="Mobile No"></v-text-field>
            </v-row>
            <h6 class="text-subtitle-1 mt-3 mb-5 ml-2 font-weight-bold">
              2. Address Details
            </h6>
            <v-row style="padding-top5px;padding-left:20px;padding-right:20px">
              <v-text-field label="House / Office No"></v-text-field
              >&nbsp;&nbsp;&nbsp;
              <v-text-field label="Apartment Name "></v-text-field
              >&nbsp;&nbsp;&nbsp;
              <v-text-field label="Street / Area"></v-text-field>
            </v-row>
            <v-row style="padding-top5px;padding-left:20px;padding-right:20px">
              <v-text-field label="City"></v-text-field>&nbsp;&nbsp;&nbsp;
              <v-text-field label="Country"></v-text-field>&nbsp;&nbsp;&nbsp;
              <v-text-field label="Pin Code"></v-text-field>
            </v-row>

            <div class="d-flex justify-end mt-12">
              <h5
                class="bg-grey-lighten-2 mr-10"
                style="padding: 10px 30px; border-radius: 5px"
              >
                Cancle
              </h5>
              <h5
                class="bg-grey-lighten-2 mr-5"
                style="padding: 10px 30px; border-radius: 5px"
              >
                Submit
              </h5>
            </div>
          </div>
        </div>
        <!-- other -->
      </div>
    </div>
    <br />
    <br />
    <br />
  </div>
</template>

<script>
export default {};
</script>

<style></style>
