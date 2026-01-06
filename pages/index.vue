<template>
  <v-container fluid>
    <v-img class="ma-auto mt-3" src="/logo.svg" width="350" contain />
    <p class="text-center mt-3">
      Affiliated to the <a href="https://www.showbudgies.co.za" target="_blank">Budgerigar
        Society of South Africa</a>
    </p>

    <SliderH />
    <SliderG />
    <SliderF />
    <SliderE />
    <SliderD />
    <SliderC />

    <v-card class="pa-3 mt-3 mb-3 text-center purple lighten-5">
      <!--      <CountDownTimer/>-->
      <a href="https://showbudgies.co.za/shows/">Click here for details and documentation.</a>
    </v-card>

    <v-btn
      block
      class="rounded-0 white--text hidden-md-and-up"
      color="purple darken-3"
      href="https://www.showbudgies.co.za/shows/"
      target="_blank"
    >
      Upcoming Shows
    </v-btn>
    <v-btn
      block
      class="rounded-0 mt-1 mb-2 white--text hidden-md-and-up"
      color="purple darken-3"
      href="https://www.showbudgies.co.za/results/results-main"
      target="_blank"
    >
      SA Show Results
    </v-btn>

    <h2 class="text-center font-weight-light purple lighten-2 white--text">
      Competition Winners
    </h2>

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
              Preggy Chetty
            </h4>
            <h4 class="text-center font-weight-light">
              <v-icon class="mb-1" small>
                mdi-cellphone
              </v-icon>
              : 083 375 4776
            </h4>
          </v-card>
        </v-col>
        <v-col cols="12" sm="3">
          <v-card class="pa-3 purple white--text rounded-0" flat>
            <h5 class="text-center">
              Treasurer
            </h5>
            <h4 class="text-center font-weight-light">
              Michael Borcherds
            </h4>
            <h4 class="text-center font-weight-light">
              <v-icon class="mb-1" small>
                mdi-cellphone
              </v-icon>
              : 082-441-7305
            </h4>
          </v-card>
        </v-col>
        <v-col cols="12" sm="3">
          <v-card class="pa-3 blue-grey white--text rounded-0" flat>
            <h5 class="text-center">
              Secretary
            </h5>
            <h4 class="text-center font-weight-light">
              Todd Young
            </h4>
            <h4 class="text-center font-weight-light">
              <v-icon class="mb-1" small>
                mdi-cellphone
              </v-icon>
              : 067 640 7504
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
    ],
    images: [
      { src: 'images/home/bird3.jpeg', title: 'Best Bird in Show - Pierre ' },
      { src: 'images/home/bird4.jpeg', title: 'Best Opposite Sex - Pierre ' },
      { src: 'images/home/bird5.jpeg', title: 'Best Intermediate + Best Derby - Henk' },
      { src: 'images/home/bird6.jpeg', title: 'Best Opposite Sex - Retha' },
      { src: 'images/home/bird7.jpeg', title: 'Best Novice - Preggy/Kaiden' },
      { src: 'images/home/bird8.jpeg', title: 'Best Novice Opposite Sex - Sarel' },
      { src: 'images/home/bird1.jpeg', title: 'Grey Green Cock Derby winner 17th Oct 2022 Pierre Swart' },
      { src: 'images/home/bird2.jpeg', title: 'Yellowface hen Derby opposite sex and best Novice 17th October 2022 Preggy&Kaiden' }
    ]
  })
}
</script>
