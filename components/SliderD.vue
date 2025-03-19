<template>
  <v-sheet
    class="mx-auto mb-3"
    elevation="0"
  >
    <h4 class="text-center purple darken-3 white--text">JSBS mini show 09 December 2023</h4>
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
      { src: 'images/minishow2023/Best Champion.jpg', show: 'JSBS mini show 09 December 2023', title: 'Best Champion/BIS', name: 'Molketin stud' },
      { src: 'images/minishow2023/Best Intermediate Opp Sex.jpg', show: 'JSBS mini show 09 December 2023', title: 'Best opposite sex Intermediate', name: 'Preggy Chetty' },
      { src: 'images/minishow2023/Best Intermediate.jpg', show: 'JSBS mini show 09 December 2023', title: 'Best intermediate', name: 'Preggy Chetty' },
      { src: 'images/minishow2023/Best Novice Opp Sex.jpg', show: 'JSBS mini show 09 December 2023', title: 'Best opposite sex novice', name: 'Sarel v Zyl' },
      { src: 'images/minishow2023/Best Novice.jpg', show: 'JSBS mini show 09 December 2023', title: 'Best Novice', name: 'Todd Young' },
      { src: 'images/minishow2023/Champion Opp Sex.jpg', show: 'JSBS mini show 09 December 2023', title: 'Best oppisite sex Champion', name: 'Molkenten' }
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
