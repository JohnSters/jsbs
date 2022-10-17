<template>
  <v-container fluid>
    <v-img class="ma-auto" src="/logo.svg" width="300"/>
    <p class="text-center mt-3">
      Affiliated to the <a href="https://www.showbudgies.co.za" target="_blank">Budgerigar
        Society of South Africa</a>
    </p>

    <v-row class="hidden-lg-and-up">
      <v-col
        v-for="(image, id) in images"
        :key="id"
        class="d-flex child-flex"
        cols="3"
      >
        <v-card class="pa-3 mb-3">
          <v-img
            :src="image.src"
            height="350"
            contain
            aspect-ratio="1"
            class="purple lighten-5"
          >
            <template v-slot:placeholder>
              <v-row
                class="fill-height ma-0"
                align="center"
                justify="center"
              >
                <v-progress-circular
                  indeterminate
                  color="grey lighten-5"
                ></v-progress-circular>
              </v-row>
            </template>
          </v-img>

          <p class="text-center mt-3">{{ image.title }} <br> <a :href="image.src" target="_blank">View Image</a> </p>

        </v-card>
      </v-col>
    </v-row>

    <v-row class="hidden-md-and-down">
      <v-col
        v-for="(image, id) in images"
        :key="id"
        class="d-flex child-flex"
        cols="3"
      >
        <v-card class="pa-3 mb-3">
          <v-img
            :src="image.src"
            height="550"
            contain
            aspect-ratio="1"
            class="purple lighten-5"
          >
            <template v-slot:placeholder>
              <v-row
                class="fill-height ma-0"
                align="center"
                justify="center"
              >
                <v-progress-circular
                  indeterminate
                  color="grey lighten-5"
                ></v-progress-circular>
              </v-row>
            </template>
          </v-img>

          <p class="text-center mt-3">{{ image.title }} <br> <a :href="image.src" target="_blank">View Image</a> </p>

        </v-card>
      </v-col>
    </v-row>

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
    ],
    images: [
      { src: 'images/home/bird3.jpeg', title: 'Best Bird in Show - Pierre ' },
      { src: 'images/home/bird4.jpeg', title: 'Best Opposite Sex - Pierre ' },
      { src: 'images/home/bird5.jpeg', title: 'Best Intermediate + Best Derby - Henk' },
      { src: 'images/home/bird6.jpeg', title: 'Best Opposite Sex - Retha' },
      { src: 'images/home/bird7.jpeg', title: 'Best Noive - Preggy/Kaiden' },
      { src: 'images/home/bird8.jpeg', title: 'Best Novice Opposite Sex - Sarel' },
      { src: 'images/home/bird1.jpeg', title: 'Grey Green Cock Derby winner 17th Oct 2022 Pierre Swart' },
      { src: 'images/home/bird2.jpeg', title: 'Yellowface hen Derby opposite sex and best Novice 17th October 2022 Preggy&Kaiden' }
    ]
  })
}
</script>
