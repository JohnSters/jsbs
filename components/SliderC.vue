<template>
  <v-sheet
    class="mx-auto mb-3"
    elevation="0"
  >
    <h4 class="text-center purple darken-3 white--text">
      2023 JSBS GP Nationals
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
      { src: 'images/gp-nationals2023/best-on-show-gpn-2023.jpg', show: 'GP Nationals', title: 'Best on show - Gauteng Nationals 2023', name: 'Molketin Stud' },
      { src: 'images/gp-nationals2023/best-opposite-sex-gpn-2023.jpg', show: 'GP Nationals', title: 'Gauteng National 2023 best opp sex on show', name: 'Pierre Swart' },
      { src: 'images/gp-nationals2023/best-color-year-gpn-2023.jpg', show: 'GP Nationals', title: 'Best color of the Year - Yellowface', name: 'Pierre Swart' },
      { src: 'images/gp-nationals2023/best-rare-on-show-gpn-2023.jpg', show: 'GP Nationals', title: 'Best Rare on Show', name: 'Pierre Swart' },
      { src: 'images/gp-nationals2023/best-clearwing-on-show-gpn-2023.jpg', show: 'GP Nationals', title: 'Best Clearwing on Show', name: 'Atom Stud' },
      { src: 'images/gp-nationals2023/best-albino-on-show-gpn-2023.jpg', show: 'GP Nationals', title: 'Best Albino On Show', name: 'Van der Heever Stud' }
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
