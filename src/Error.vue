<template>
<v-ons-page>
  <h1 class="er_code_text">404</h1>
  <p class="er_text">This page does not exist.</p>
  <div class="er_details_text">
    <router-link to="/">Go to Home</router-link>
  </div>
</v-ons-page>
</template>

<style scoped>
.er_code_text {
  font-size: 60px;
  color: #555;
  text-align: center;
}

.er_text {
  font-size: 15px;
  color: gray;
  text-align: center;
}

.er_details_text {
  text-align: center;
}
</style>