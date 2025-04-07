<template>
  <v-sheet
    class="mx-auto mb-3"
    elevation="0"
  >
    <h4 class="text-center purple darken-3 white--text">JSBS February Show</h4>
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
      { src: 'images/feb-club-show/Best Novice.jpg', show: 'February Club Show 2025', title: 'Best Novice', name: 'Attie Van Staaden' },
      { src: 'images/feb-club-show/Champion opposite sex.jpg', show: 'February Club Show 2025', title: 'Champion opposite sex', name: 'Mike Davies' },
      { src: 'images/feb-club-show/Novice opposite sex.jpg', show: 'February Club Show 2025', title: 'Novice opposite sex', name: 'Nathan Bosch' },
      { src: 'images/feb-club-show/Best Champion.jpg', show: 'February Club Show 2025', title: 'Best Champion', name: 'Mike Davies' },
      { src: 'images/feb-club-show/Best in ShowBest Intermediate.jpg', show: 'February Club Show 2025', title: 'Best in Show/Best Intermediate', name: 'Todd Young' },
      { src: 'images/feb-club-show/best-opposite.jpg', show: 'February Club Show 2025', title: 'Best Opposite', name: 'Todd Young ' }
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
