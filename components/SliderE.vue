<template>
  <v-sheet
    class="mx-auto mb-3"
    elevation="0"
  >
    <h4 class="text-center purple darken-3 white--text">JSBS mini show 13 April 2024</h4>
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
  name: 'SliderB',
  data: () => ({
    model: null,
    items: [
      { src: 'images/minishow2024/best-albino-on-show.jpg', show: '13 April 2024', title: 'Best Albino on Show', name: 'Ronnie Riep' },
      { src: 'images/minishow2024/best-violet-on-show.jpg', show: '13 April 2024', title: 'Best Violet on Show, Best Champion', name: 'Marius Heydenrych' },
      { src: 'images/minishow2024/best-suffused.jpg', show: '13 April 2024', title: 'Best suffused', name: 'Todd Young' },
      { src: 'images/minishow2024/best-opposite-sex.jpg', show: '13 April 2024', title: 'Best opposite sex rare, Best Rec Pied', name: 'PC Birds' },
      { src: 'images/minishow2024/runner-up-to-best-rare.jpg', show: '13 April 2024', title: 'Runner up to Best Rare, Best Texas Clearbody', name: 'PC Birds' },
      { src: 'images/minishow2024/best-rare-on-show.jpg', show: '13 April 2024', title: 'Best Rare on Show, Best  Golden Face, Best Novice', name: 'Todd Young' }
    ]
  })
}
</script>

<style lang="css" scoped >
.v-slide-group__next, .v-slide-group__prev {
  min-width: 30px !important;
  background: palegoldenrod;
  height: 375px;
  margin-top: 4px;
  max-width: 100px;
}
</style>
