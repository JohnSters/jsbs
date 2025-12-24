<template>
  <v-container>
    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text>
        <v-icon class="mr-2">
          mdi-arrow-left
        </v-icon>Main Menu
      </v-btn>
      <v-btn to="/mini/MiniShow2019" class="purple darken-1" dark rounded text>
        Mini Show 2019<v-icon class="ml-2">
          mdi-arrow-right
        </v-icon>
      </v-btn>
    </div>

    <h1>Mini Show Results 2022</h1>

    <v-simple-table>
      <template #default>
        <thead>
          <tr>
            <th class="text-left">
              Mini Show Date
            </th>
            <th class="text-left">
              Award
            </th>
            <th class="text-left">
              Exhibitor
            </th>
            <th class="text-left">
              Status
            </th>
          </tr>
        </thead>
        <tbody>
          <tr
            v-for="item in mini2022"
            :key="item.name"
          >
            <td>{{ item.date }}</td>
            <td>{{ item.award }}</td>
            <td>{{ item.exh }}</td>
            <td>{{ item.status }}</td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-divider class="ma-3 purple" />

    <v-row class="mt-3">
      <v-col v-for="(item, index) in items" :key="index" cols="12" sm="4">
        <v-card class="pa-3">
          <v-img :src="item.src" height="400" contain />
          <p class="mt-1 text-center">
            {{ item.title }} <br> {{ item.name }}
          </p>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2022',
  data () {
    return {
      mini2022: [
        { date: '19 November 2022', award: 'Best Bird on Show (Online Show)', exh: 'Imran Majiet', status: 'Intermediate (Online Show)' },
        { date: '.', award: 'Best Champion on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Pierre Swart', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show Novice', exh: 'Sarel Nortje', status: 'Novice' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Henk Potgieter', status: 'Intermediate' },
        { date: '.', award: 'Best Novice on Show', exh: 'Sarel Nortje', status: 'Novice' }
      ],
      items: [
        { src: '/images/minishow2022/best-show.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best in Show', name: 'Imran Majiet (online show)' },
        { src: '/images/minishow2022/best-derby.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best in Show and Best Champion', name: 'Molkentin Stud' },
        { src: '/images/minishow2022/best-intermediate.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best Intermediate', name: 'Henk Potgieter' },
        { src: '/images/minishow2022/best-novice.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best Novice', name: 'Sarel Nortje' },
        { src: '/images/minishow2022/opposite-sex.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best Opposite sex', name: 'Sarel Nortje' },
        { src: '/images/minishow2022/opposite-sex2.jpeg', show: 'JSBS Mini show held 19 November 2022', title: 'Best Opposite sex', name: 'Pierre Swart' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
