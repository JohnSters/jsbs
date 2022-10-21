<template>
  <v-container>

    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text><v-icon class="mr-2">mdi-arrow-left</v-icon>Main Menu</v-btn>
      <v-btn to="/mini/MiniShow2009" class="purple darken-1" dark rounded text>Mini Show 2009 <v-icon class="ml-2">mdi-arrow-right</v-icon></v-btn>
    </div>

    <h1>Mini Show Results 2010</h1>

    <v-simple-table>
      <template v-slot:default>
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
          v-for="item in mini2019"
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

    <v-row class="mt-6">
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2010/ms1101.jpg" height="400" contain></v-img>
        Best Bird on Show - Clarence Marks
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2010/ms1102.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Grobbelaar Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2010/ms1103.jpg" height="400" contain></v-img>
        Best Champion on Show - Nel Brothers Stud
      </v-col>
    </v-row>

  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2010',
  data () {
    return {
      mini2019: [
        { date: '10 July 2010', award: 'Best Bird on Show', exh: 'Clarence Marks', status: 'Novice' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Grobbelaar Stud', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Clarence Marks', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '14 August 2010', award: 'Best Bird on Show', exh: 'Gert Pieters', status: 'Intermediate' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Danie Bisschoff', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'Smartryk Burger', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Danie Bisschoff', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
