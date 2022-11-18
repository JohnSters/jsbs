<template>
  <v-container fluid>
    <v-card-title class="text-center justify-center py-6 hidden-md-and-up">
      <h2 class="font-weight-bold basil--text">
        JSBS Sales
      </h2>
    </v-card-title>

    <v-card-title class="text-center justify-center py-6 hidden-sm-and-down">
      <h3 class="font-weight-bold text-h2 basil--text">
        JSBS Sales
      </h3>
    </v-card-title>
    <v-row>
      <v-col cols="12" sm="4">
        <v-card class="pa-6" shaped>
          <v-img class="ma-auto" src="/images/logo-round.png" width="200" contain></v-img>
          <p class="mt-6"><b>Iodine/Calcium Bird Blocks for sale</b></p>
          <p>Give your birds all the necessary Minerals/Vitamins they need all year. Increase bone strength, less egg bound, increase egg strength, increase general health of your birds.</p>
          <v-btn href="https://www.mbsb.co.za/" target="_blank" class="red" dark>Order Now!</v-btn>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'SalesPage'
}
</script>

<style scoped>

</style>
