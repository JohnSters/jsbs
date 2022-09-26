<template>
  <v-container fluid>
    <v-img class="ma-auto" src="/logo.svg" width="339" />
    <p class="text-center mt-3">
      Affiliated to the <a href="https://www.showbudgies.co.za" target="_blank">Budgerigar
        Society of South Africa</a>
    </p>

    <v-carousel v-model="model">
      <v-carousel-item
        v-for="(color, i) in colors"
        :key="color"
      >
        <v-sheet
          :color="color"
          height="100%"
          tile
        >
          <v-row
            class="fill-height"
            align="center"
            justify="center"
          >
            <div class="text-h2">
              Slide {{ i + 1 }}
            </div>
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel>

    <v-card class="pa-3" flat>
      <h2 class="blue-grey--text text-center mt-3">
        ON BEHALF OF THE BSSA MC.
      </h2>
      <h3 class="font-weight-light blue-grey--text text-center">
        It is with great pride to announce that <b
          class="font-weight-bold"
        >Reinhard Molkentin</b> has won the
        <br>WBO 2021
        <b>Gould</b> Award.
      </h3>
      <v-img class="ma-auto" src="/images/reinhard.png" width="350" />
      <h3 class="font-weight-light blue-grey--text text-center mt-3">
        "Congratulations to Reinhard on this prestigious
        award."
      </h3>
    </v-card>

    <v-card class="text-center pa-3 mt-3 mb-6 blue-grey--text" flat>
      <h2 class="blue-grey--text font-weight-bold">
        Important BSSA Notice
      </h2>

      <p>
        It's with great personal sadness to announce that Reinhard Molkentin passed away this morning 10 August 2022
        at the age of 83. He was a colossus in the budgie fancy all over the world.
      </p>
      <br>
      <h3 class="black--text">
        Rest In Peace Reinhard, Auf Wiedersehen!!
      </h3>
    </v-card>

    <v-card class="pa-6" flat>
      <v-row>
        <v-col cols="12" sm="3">
          <v-card class="pa-3 blue-grey white--text rounded-0" flat>
            <h5 class="text-center">
              Chairman
            </h5>
            <h4 class="text-center font-weight-light">
              Pierre Swart
            </h4>
            <h4 class="text-center font-weight-light">
              <v-icon class="mb-1" small>
                mdi-cellphone
              </v-icon>
              : 079-797-5265
            </h4>
          </v-card>
        </v-col>
        <v-col cols="12" sm="3">
          <v-card class="pa-3 purple white--text rounded-0" flat>
            <h5 class="text-center">
              Vice Chairmen
            </h5>
            <h4 class="text-center font-weight-light">
              Mike Davies
            </h4>
            <h4 class="text-center font-weight-light">
              <v-icon class="mb-1" small>
                mdi-cellphone
              </v-icon>
              : 082-056-4734
            </h4>
          </v-card>
        </v-col>
        <v-col cols="12" sm="3">
          <v-card class="pa-3 purple white--text rounded-0" flat>
            <h5 class="text-center">
              Treasurer
            </h5>
            <h4 class="text-center font-weight-light">
              Morne Bothma
            </h4>
            <h4 class="text-center font-weight-light">
              <v-icon class="mb-1" small>
                mdi-cellphone
              </v-icon>
              : 082-867-4352
            </h4>
          </v-card>
        </v-col>
        <v-col cols="12" sm="3">
          <v-card class="pa-3 blue-grey white--text rounded-0" flat>
            <h5 class="text-center">
              Secretary
            </h5>
            <h4 class="text-center font-weight-light">
              Retha van Deventer
            </h4>
            <h4 class="text-center font-weight-light">
              <v-icon class="mb-1" small>
                mdi-cellphone
              </v-icon>
              : 082-685-7139
            </h4>
          </v-card>
        </v-col>
      </v-row>
    </v-card>
  </v-container>
</template>

<script>
export default {
  name: 'IndexPage',
  data: () => ({
    model: 0,
    colors: [
      'primary',
      'secondary',
      'yellow darken-2',
      'red',
      'orange'
    ]
  })
}
</script>
