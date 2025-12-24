<template>
  <v-container>
    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text>
        <v-icon class="mr-2">
          mdi-arrow-left
        </v-icon>Main Menu
      </v-btn>
      <v-btn to="/mini/MiniShow2008" class="purple darken-1" dark rounded text>
        Mini Show 2008 <v-icon class="ml-2">
          mdi-arrow-right
        </v-icon>
      </v-btn>
    </div>

    <h1>Mini Show Results 2009</h1>

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
        <v-img src="/images/budgies/minishow2009/ms1091.jpg" height="400" contain />
        Best Bird on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2009/ms1092.jpg" height="400" contain />
        Best Opposite Sex on Show - Gert Pieters
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2009/ms1093.jpg" height="400" contain />
        Best Novice on Show - Clarence Marks
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2009/ms2091.jpg" height="400" contain />
        Best Bird on Show - Mike Davies
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2009/ms2091.jpg" height="400" contain />
        Best Opposite Sex on Show - Gert Pieters
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2009',
  data () {
    return {
      mini2019: [
        { date: '18 April 2009', award: 'Best Bird on Show', exh: 'Nel Brothers Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Gert Pieters', status: 'Intermediate' },
        { date: '.', award: 'Best Champion on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Clarence Marks', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '9 May 2009', award: 'Best Bird on Show', exh: 'Mike Davies', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Gert Pieters', status: 'Intermediate' },
        { date: '.', award: 'Best Champion on Show', exh: 'Mike Davies', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Christo Grobbelaar', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '18 July 2009', award: 'Best Bird on Show', exh: 'Mike Davies', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Gert Pieters', status: 'Intermediate' },
        { date: '.', award: 'Best Champion on Show', exh: 'Mike Davies', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Clarence Marks', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '15 August 2009', award: 'Best Bird on Show', exh: 'Gert Pieters', status: 'Intermediate' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Mike Davies', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Mike Davies', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Grobbelaar Stud', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
