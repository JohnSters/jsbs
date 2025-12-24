<template>
  <v-container fluid>
    <v-card-title class="text-center justify-center py-6 hidden-md-and-up">
      <h2 class="font-weight-bold basil--text">
        The Society
      </h2>
    </v-card-title>

    <v-card-title class="text-center justify-center py-6 hidden-sm-and-down">
      <h3 class="font-weight-bold text-h2 basil--text">
        The Society
      </h3>
    </v-card-title>

    <v-tabs
      v-model="tab"
      color="purple"
      grow
    >
      <v-tab>
        Upcoming Events
      </v-tab>
      <v-tab>
        Membership Fees
      </v-tab>
      <v-tab>
        Society Guidelines
      </v-tab>
      <v-tab>
        Year Program
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item>
        <v-card
          color="basil"
          flat
        >
          <v-card class="ma-1 mt-2 pa-3 text-center">
            <CountDownTimer />
            <h2>Venue: Attie Van Staden’s Residence</h2>
            <p>email: Leonard @ <b>Govenderleonard98@gmail.com</b> for more info.</p>
          </v-card>
          <v-card class="ma-1 pa-3">
            Other Upcoming Events
            <ul>
              <li>JSBS Derby birds 1 to 20 of 2022</li>
              <li>JSBS Club show all 2022 rung birds eligible</li>
              <li>Judge for the day will be announced</li>
            </ul>
          </v-card>
        </v-card>
      </v-tab-item>

      <v-tab-item>
        <v-card
          color="basil"
          flat
        >
          <v-card-text>
            If you are interested in Show Budgies and would like to know more about this interesting hobby
            and would like to contact your nearest club in South Africa.
            <br>
            <br>
            <h3>Email Leonard @ <b>Govenderleonard98@gmail.com</b></h3>

            <h3 class="mt-3">
              Club Fees: R450, Affiliation Fees: R500
            </h3>
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
            7. Membership fees must be paid-up by the end of August, before the Annual General Meeting, in order for
            ring orders to be processed.
          </v-card-text>
        </v-card>
      </v-tab-item>
      <v-tab-item>
        <v-card>
          <h3>Important Dates</h3>
          <p>
            The JSBS year program is set up at the beginning of each year so that all members can diarise these dates.
            Year program is included in each months Monthly Minutes.
          </p>
          <ul>
            <li>16 July - First Ring order date for next years rings</li>
            <li>31 August - JSBS subs due for next year</li>
            <li>1 September - Final date for current year ring orders</li>
            <li>BSSA Management Committee Nominations due 3 months before the National Show.</li>
          </ul>
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
