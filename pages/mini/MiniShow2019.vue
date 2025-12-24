<template>
  <v-container>
    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1 mt-2" dark rounded text>
        <v-icon class="mr-2">
          mdi-arrow-left
        </v-icon>Main Menu
      </v-btn>
      <v-btn to="/mini/MiniShow2018" class="purple darken-1 mt-2" dark rounded text>
        Mini Show 2018 <v-icon class="ml-2">
          mdi-arrow-right
        </v-icon>
      </v-btn>
    </div>

    <h1>Mini Show Results 2019</h1>

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
  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2019',
  data () {
    return {
      mini2019: [
        { date: '19 January 2019', award: 'Best Bird on Show', exh: 'Pierre Swart', status: 'Champion' },
        { date: '.', award: 'Best Opp`osite Sex on Show', exh: 'Pierre Swart', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Pierre Swart', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Retha van Deventer', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'None', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '26 October 2019', award: 'Best Bird on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Molkentin Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Retha van Deventer', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'The Grey Stud', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
