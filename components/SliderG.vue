<template>
  <v-sheet
    class="mx-auto mb-3"
    elevation="0"
  >
    <h4 class="text-center purple darken-3 white--text">
      Derby Show 2025
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
          :src="item.src"
          class="ma-1"
          height="375"
          width="220"
          aspect-ratio="0.587"
          contain
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
  name: 'SliderG',
  data: () => ({
    model: null,
    items: [
      { src: 'images/derby2025/best-opposite-sex.jpg', show: 'Derby Show 2025', title: 'Best Opposite Sex', name: 'Henk Potgieter' },
      { src: 'images/derby2025/best-in-show.jpg', show: 'Derby Show 2025', title: 'Best in Show', name: 'Michael Borcherds' },
      { src: 'images/minishow2026/image1.jpg', show: 'Derby Show 2025', title: 'Best in Show and Best Intermediate', name: 'Todd Young' },
      { src: 'images/minishow2026/image2.jpg', show: 'Derby Show 2025', title: 'Best Opposite Sex and Best Champion', name: 'Mike Davies' },
      { src: 'images/minishow2026/image3.jpg', show: 'Derby Show 2025', title: 'Best Novice', name: 'Izak Visagie' }
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
