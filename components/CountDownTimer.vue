<template>
  <v-container>
    <script src="https://cdn.logwork.com/widget/countdown.js"></script>
    <a href="https://logwork.com/countdown-y6xw" class="countdown-timer" data-timezone="Africa/Johannesburg" data-date="2023-04-15 09:32">The 2023 GP Championship Show</a>
  </v-container>
</template>

<script>
export default {
  name: 'CountDownTimer',
  beforeMount () {
    if (!window.location.hash) {
      window.location = window.location + '#loaded'
      window.location.reload()
    }
  }
}
</script>

<style scoped>

</style>
