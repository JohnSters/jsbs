<template>
  <v-app>
    <MainAppBar />
    <v-main>
      <v-container fluid>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer>
      <span>&copy; 2023 Jacaranda Show Budgie Society</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {}
  }
}
</script>
