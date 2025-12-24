<template>
  <v-container>
    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text>
        <v-icon class="mr-2">
          mdi-arrow-left
        </v-icon>Main Menu
      </v-btn>
      <v-btn to="/mini/MiniShow2015" class="purple darken-1" dark rounded text>
        Mini Show 2015 <v-icon class="ml-2">
          mdi-arrow-right
        </v-icon>
      </v-btn>
    </div>

    <h1>Mini Show Results 2016</h1>

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

    <v-row class="mt-6">
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2016/ms11603.jpg" height="400" contain />
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2016/ms21601.jpg" height="400" contain />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2016',
  data () {
    return {
      mini2019: [
        { date: '22 October 2016', award: 'Best Bird on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Mike Davies', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Molkentin Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Rynier Burger', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: '-', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '14 August 2016', award: 'Best Bird on Show', exh: 'Exhibitor', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Pierre Swart', status: 'Intermediate' },
        { date: '.', award: 'Best Champion on Show', exh: 'Rynier Burger', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Pierre Swart', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Ryan vd Heever', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '9 January 2016', award: 'Best Bird on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Molkentin Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'None', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Ryan vd Heever', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
