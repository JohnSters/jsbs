<template>
  <v-sheet
    class="mx-auto mb-3"
    elevation="0"
  >
    <h4 class="text-center purple darken-3 white--text">Competition Winners</h4>
    <v-slide-group
      v-model="model"
      show-arrows
      center-active
    >
      <v-slide-item
        v-for="(item, index) in items"
        :key="index"
        v-slot="{ active, toggle }"
      >
        <v-img
          :color="active ? 'primary' : 'grey lighten-1'"
          :src="item.src"
          class="ma-1"
          height="375"
          width="220"
          @click="toggle"
        >
          <v-row
            class="fill-height"
            align="center"
            justify="center"
          >
            <v-scale-transition>
              <v-icon
                v-if="active"
                color="white"
                size="40"
                v-text="'mdi-trophy'"
              ></v-icon>
            </v-scale-transition>
          </v-row>
        </v-img>
      </v-slide-item>
    </v-slide-group>

    <v-expand-transition>
      <v-sheet
        v-if="model != null"
        height="160"
        tile
        class=""
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <h3 class="text-center hidden-sm-and-down blue-grey--text">
            {{ items[model].show }} <br>
            {{ items[model].title }} | <a :href=items[model].src target="_blank">View Image</a> <br>
            {{ items[model].name }}
          </h3>
          <h4 class="text-center hidden-md-and-up blue-grey--text">
            {{ items[model].show }} <br>
            {{ items[model].title }} <br>
            {{ items[model].name }}
          </h4>
        </v-row>
      </v-sheet>
    </v-expand-transition>
  </v-sheet>
</template>

<script>
export default {
  name: 'HomeSlider',
  data: () => ({
    model: null,
    items: [
      { src: 'images/minishow2024/best-albino-on-show.jpg', show: '13 April 2024', title: 'Best Albino on Show', name: 'Ronnie Riep' },
      { src: 'images/minishow2024/best-violet-on-show.jpg', show: '13 April 2024', title: 'Best Violet on Show, Best Champion', name: 'Marius Heydenrych' },
      { src: 'images/minishow2024/best-suffused.jpg', show: '13 April 2024', title: 'Best suffused', name: 'Todd Young' },
      { src: 'images/minishow2024/best-opposite-sex.jpg', show: '13 April 2024', title: 'Best opposite sex rare, Best Rec Pied', name: 'PC Birds' },
      { src: 'images/minishow2024/runner-up-to-best-rare.jpg', show: '13 April 2024', title: 'Runner up to Best Rare, Best Texas Clearbody', name: 'PC Birds' },
      { src: 'images/minishow2024/best-rare-on-show.jpg', show: '13 April 2024', title: 'Best Rare on Show, Best  Golden Face, Best Novice', name: 'Todd Young' },

      { src: 'images/home/2023 SA National Best Bird - Molkentin Stud.jpg', show: 'SA National', title: '2023 SA National Best Bird', name: 'Molkentin Stud' },
      { src: 'images/home/2023 SA National Best Opposite sex - Pierre Swart.jpg', show: 'SA National', title: 'SA National Best Opposite sex', name: 'Pierre Swart' },
      { src: 'images/home/BNYP.jpg', show: 'SA National', title: 'Best Novice EC area show', name: 'Munzir Patel' },
      { src: 'images/home/BYBPS.jpg', show: 'SA National', title: 'Best Young bird EC area show', name: 'Pierre Swart' },

      { src: 'images/minishow2022/best-show.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best in Show (Online Show)', name: 'Imran Majiet (online show)' },
      { src: 'images/minishow2022/best-derby.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best in Show and Best Champion', name: 'Molkentin Stud' },
      { src: 'images/minishow2022/best-intermediate.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best Intermediate', name: 'Henk Potgieter' },
      { src: 'images/minishow2022/best-novice.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best Novice', name: 'Sarel Nortje' },
      { src: 'images/minishow2022/opposite-sex2.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best Opposite sex', name: 'Pierre Swart' },
      { src: 'images/minishow2022/opposite-sex.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best Opposite Sex Novice', name: 'Sarel Nortje' },

      { src: 'images/derby2022/best-derby.jpeg', show: 'Derby Show', title: 'Best Derby on show', name: 'Pierre Swart' },
      { src: 'images/derby2022/best-intermediate.jpeg', show: 'Derby Show', title: 'Best Intermediate', name: 'Retha van Deventer' },
      { src: 'images/derby2022/best-novice.jpeg', show: 'Derby Show', title: 'Best Derby Novice', name: 'Sarel v Zyl' },
      { src: 'images/derby2022/best-sex.jpeg', show: 'Derby Show', title: 'Best Opposite sex', name: 'Preggy Chetty' },

      { src: 'images/home/bird3.jpeg', show: 'Oct Derby Show 2022', title: 'Best Bird in Show', name: 'Pierre' },
      { src: 'images/home/bird4.jpeg', show: 'Oct Derby Show 2022', title: 'Best Opposite Sex', name: 'Pierre' },
      { src: 'images/home/bird5.jpeg', show: 'Oct Derby Show 2022', title: 'Best Intermediate + Best Derby', name: 'Henk' },
      { src: 'images/home/bird6.jpeg', show: 'Oct Derby Show 2022', title: 'Best Opposite Sex', name: 'Retha' },
      { src: 'images/home/bird7.jpeg', show: 'Oct Derby Show 2022', title: 'Best Novice', name: 'Preggy/Kaiden' },
      { src: 'images/home/bird8.jpeg', show: 'Oct Derby Show 2022', title: 'Best Novice Opposite Sex', name: 'Sarel' },
      { src: 'images/home/bird1.jpeg', show: 'Oct Derby Show 2022', title: 'Grey Green Cock Derby winner', name: 'Pierre' },
      { src: 'images/home/bird2.jpeg', show: 'Oct Derby Show 2022', title: 'Yellowface hen Derby opposite sex and best Novic', name: 'Preggy&Kaiden' }
    ]
  })
}
</script>

<style lang="css" scoped >
>>> .v-slide-group__next, >>> .v-slide-group__prev {
  min-width: 30px !important;
  background: palegoldenrod;
  height: 375px;
  margin-top: 4px;
  max-width: 100px;
}
</style>
