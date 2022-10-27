<template>
  <v-container>
    <script src="https://cdn.logwork.com/widget/countdown.js"></script>
    <a class="countdown-timer"
       data-date="2022-11-19 10:00"
       data-timezone="Africa/Johannesburg"
       href="https://logwork.com/countdown-wko7"
    >JSBS Year End Function Show</a>
  </v-container>
</template>

<script>
export default {
  name: 'CountDownTimer',
  mounted () {
    if (!window.location.hash) {
      window.location = window.location + '#loaded'
      window.location.reload()
    }
  }
}
</script>

<style scoped>

</style>
