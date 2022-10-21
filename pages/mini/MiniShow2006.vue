<template>
  <v-container>

    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text><v-icon class="mr-2">mdi-arrow-left</v-icon>Main Menu</v-btn>
      <v-btn to="/mini/MiniShow2005" class="purple darken-1" dark rounded text>Mini Show 2005 <v-icon class="ml-2">mdi-arrow-right</v-icon></v-btn>
    </div>

    <h1>Mini Show Results 2006</h1>

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
        <v-img src="/images/budgies/minishow2006/ms1061.jpg" height="400" contain></v-img>
        Best Champion Opposite Sex - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2006/ms1062.jpg" height="400" contain></v-img>
        Best Novice and Best Opposite Sex on Show - Clarence Marks
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2006/ms1063.jpg" height="400" contain></v-img>
        Best Bird on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2006/ms1066.jpg" height="400" contain></v-img>
        Best Intermediate on Show - Gert Pieters
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2006/ms2061.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Gert Pieters
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2006/ms2062.jpg" height="400" contain></v-img>
        Best Bird on Show - Gert Pieters
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2006/ms3061.jpg" height="400" contain></v-img>
        Best Bird on Show and Best Champion on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2006/ms3062.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2006/ms3063.jpg" height="400" contain></v-img>
        Best Intermediate on Show - Gert Pieters
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2006/ms4061.jpg" height="400" contain></v-img>
        Best Bird on Show - Clarence Marks
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2006/ms4063.jpg" height="400" contain></v-img>
        Best Intermediate on Show - Gert Pieters
      </v-col>
    </v-row>

  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2006',
  data () {
    return {
      mini2019: [
        { date: '11 March 2006', award: 'Best Bird on Show', exh: 'Nel Brothers Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Clarence Marks', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Clarence Marks', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '20 May 2006', award: 'Best Bird on Show', exh: 'Gert Pieters', status: 'Intermediate' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Gert Pieters', status: 'Intermediate' },
        { date: '.', award: 'Best Champion on Show', exh: 'Pieter van der Linde', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Clarence Marks', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '26 August 2006', award: 'Best Bird on Show', exh: 'Nel Brothers Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Clarence Marks', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '14 October 2006', award: 'Best Bird on Show', exh: 'Clarence Marks', status: 'Novice' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Mike Davies', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Clarence Marks', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
