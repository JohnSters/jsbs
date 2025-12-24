<template>
  <v-container>
    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text>
        <v-icon class="mr-2">
          mdi-arrow-left
        </v-icon>Main Menu
      </v-btn>
      <v-btn to="/mini/MiniShow2013" class="purple darken-1" dark rounded text>
        Mini Show 2013 <v-icon class="ml-2">
          mdi-arrow-right
        </v-icon>
      </v-btn>
    </div>

    <h1>Mini Show Results 2014</h1>

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
        <v-img src="/images/budgies/minishow2014/ms11401.jpg" height="400" contain />
        Best Bird on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2014/ms11402.jpg" height="400" contain />
        Best Novice on Show - Bill Stanley
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2014/ms21402.jpg" height="400" contain />
        Best Bird on Show - Mike Davies
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2014/ms21403.jpg" height="400" contain />
        Best Opposite Sex on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2014/ms21404.jpg" height="400" contain />
        First Natural to win Best Bird on Show (JSBC) - Mike Davies
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2014',
  data () {
    return {
      mini2019: [
        { date: '15 March 2014', award: 'Best Bird on Show', exh: 'Nel Brothers Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'None', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Bill Stanley', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '16 August 2014', award: 'Best Bird on Show', exh: 'Mike Davies', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Mike Davies', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'None', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'None', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
