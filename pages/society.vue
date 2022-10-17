<template>
  <v-container>
    <v-card-title class="text-center justify-center py-6">
      <h1 class="font-weight-bold text-h2 basil--text">
        The Society
      </h1>
    </v-card-title>

    <v-tabs
      v-model="tab"
      color="purple"
      grow
    >
      <v-tab>
        Membership Fees
      </v-tab>
      <v-tab>
        Society Guidelines
      </v-tab>
      <v-tab>
        Next
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item>
        <v-card
          color="basil"
          flat
        >
          <v-card-text>
            If you are interested in Show Budgies and would like to know more about this interesting hobby
            and would like to contact your nearest club in South Africa.
            <br>
            email: <b>retha@tbgequine.co.za</b>

            <h3 class="mt-3">Club Fees: R450, Affiliation Fees: R500</h3>
          </v-card-text>
        </v-card>
      </v-tab-item>

      <v-tab-item>
        <v-card
          color="basil"
          flat
        >
          <v-card-text>
            1. Applications must undertake the following
            <br>
            2. Be active by attending and partaking in as many shows as possible by...
            <br>
            <br>
            <ul>
              <li><b>Exhibiting</b></li>
              <li><b>Helping with shows</b></li>
              <li><b>Providing Financial Assistance</b></li>
              <li><b>Judging at shows</b></li>
              <li><b>Being available when help is requested</b></li>
            </ul>
            <br>
            3. Attend as many monthly meetings as possible
            <br>
            4. Make every effort to attend the annual general meeting
            <br>
            5. Support and attend club functions like aviary visits, Mini shows, etc.
            <br>
            6. Help and assist all club members.
            <br>
            7. Membership fees must be paid-up by the end of August, before the Annual General Meeting, in order for ring orders to be processed.
          </v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-container>
</template>

<script>
export default {
  name: 'SocietyPage',
  data: () => ({
    tab: null
  })
}
</script>

<style scoped>

</style>
