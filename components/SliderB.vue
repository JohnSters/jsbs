<template>
  <v-sheet
    class="mx-auto mb-3"
    elevation="0"
  >
    <h4 class="text-center purple darken-3 white--text">
      2023 JSBS Gauteng Show
    </h4>
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
              />
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
            {{ items[model].title }} | <a :href="items[model].src" target="_blank">View Image</a> <br>
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
  name: 'SliderB',
  data: () => ({
    model: null,
    items: [
      { src: 'images/gp-show/champion.jpeg', show: '2023 JSBS Gauteng Show', title: 'Best Bird on Show, Best Champion on Show, Best Any Age on Show', name: 'Molkentin Stud - Cinnamon Sky Blue' },
      { src: 'images/gp-show/runner-up-tbb.jpeg', show: '2023 JSBS Gauteng Show', title: 'Runner-up to Best Bird', name: 'Lutino Cock - Molkentin Stud' },
      { src: 'images/gp-show/best-young-bird.jpeg', show: '2023 JSBS Gauteng Show', title: 'Best Young Bird on Show', name: 'Molkentin Stud' },
      { src: 'images/gp-show/best-spangle.jpeg', show: '2023 JSBS Gauteng Show', title: 'Best Spangle on Show ', name: 'Molkentin Stud' },
      { src: 'images/gp-show/best-rare.jpeg', show: '2023 JSBS Gauteng Show', title: 'Best Rare on Show', name: 'Molkentin Stud' },
      { src: 'images/gp-show/best-boc.jpeg', show: '2023 JSBS Gauteng Show', title: 'Best BOC', name: 'Sarel Van Zyl' },
      { src: 'images/gp-show/recesive-pied.jpeg', show: '2023 JSBS Gauteng Show', title: 'Recessive Pied CC', name: 'PC birds' },
      { src: 'images/gp-show/suffuse-cc.jpeg', show: '2023 JSBS Gauteng Show', title: 'Suffuse CC', name: 'Pierre Swart' },
      { src: 'images/gp-show/fallow-cc.jpeg', show: '2023 JSBS Gauteng Show', title: 'Fallow CC', name: 'PC Birds' },
      { src: 'images/gp-show/crest-cc.jpeg', show: '2023 JSBS Gauteng Show', title: 'Crest CC', name: 'Molketin stud' },
      { src: 'images/gp-show/texas-clearbody.jpeg', show: '2023 JSBS Gauteng Show', title: 'Texas Clearbody', name: 'Molketin Stud' },
      { src: 'images/gp-show/dominent-pied.jpeg', show: '2023 JSBS Gauteng Show', title: 'Dominant Pied CC', name: 'Pierre Swart' },
      { src: 'images/gp-show/easley-clearbody.jpeg', show: '2023 JSBS Gauteng Show', title: 'Easley Clearbody CC', name: 'Pierre Swart' },
      { src: 'images/gp-show/lacewing-cc.jpeg', show: '2023 JSBS Gauteng Show', title: 'Lacewing CC', name: 'Pierre Swart' },
      { src: 'images/gp-show/clearwing-cc.jpeg', show: '2023 JSBS Gauteng Show', title: 'Clearwing CC', name: 'ATOM Stud' },
      { src: 'images/gp-show/double-factor-spangle.jpeg', show: '2023 JSBS Gauteng Show', title: 'Double Factor Spangle CC', name: 'Molketin stud' },
      { src: 'images/gp-show/cinnamon-spangle.jpeg', show: '2023 JSBS Gauteng Show', title: 'Cinnamon Spangle Series CC', name: 'Molketin stud' },
      { src: 'images/gp-show/opeline-blue.jpeg', show: '2023 JSBS Gauteng Show', title: 'Opaline Blue Series CC', name: 'Pierre Swart' },
      { src: 'images/gp-show/lutino-cc.jpeg', show: '2023 JSBS Gauteng Show', title: 'Lutino CC', name: 'Molketin stud' },
      { src: 'images/gp-show/cinnamon-grey.jpeg', show: '2023 JSBS Gauteng Show', title: 'Cinnamon Grey CC', name: 'Molketin stud' },
      { src: 'images/gp-show/cinnamon-grey-green.jpeg', show: '2023 JSBS Gauteng Show', title: 'Cinnamon Grey Green CC', name: 'Molketin stud' },
      { src: 'images/gp-show/cinnamon-green.jpeg', show: '2023 JSBS Gauteng Show', title: 'Cinnamon Green CC', name: 'Molketin Stud' },
      { src: 'images/gp-show/grey-green-cc.jpeg', show: '2023 JSBS Gauteng Show', title: 'Grey Green CC', name: 'Pierre Swart' }
    ]
  })
}
</script>

<style lang="css" scoped>
.v-slide-group__next, .v-slide-group__prev {
  min-width: 30px !important;
  background: palegoldenrod;
  height: 375px;
  margin-top: 4px;
  max-width: 100px;
}
</style>
