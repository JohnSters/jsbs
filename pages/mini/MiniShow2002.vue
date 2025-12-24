<template>
  <v-container>
    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text>
        <v-icon class="mr-2">
          mdi-arrow-left
        </v-icon>Main Menu
      </v-btn>
      <v-btn to="/mini/MiniShow2001" class="purple darken-1" dark rounded text>
        Mini Show 2001 <v-icon class="ml-2">
          mdi-arrow-right
        </v-icon>
      </v-btn>
    </div>

    <h1>Mini Show Results 2002</h1>

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
        <v-img src="/images/budgies/minishow2002/ms1021.jpg" height="400" contain />
        Best Bird on Show - Deon Davie
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms1022.jpg" height="400" contain />
        Best Intermediate on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms2021.jpg" height="400" contain />
        Best Bird on Show - Molkentin Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms2023.jpg" height="400" contain />
        Best Intermediate on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms3021.jpg" height="400" contain />
        Best Bird on Show - Deon Davie
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms3022.jpg" height="400" contain />
        Best Intermediate on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms3023.jpg" height="400" contain />
        Best Opposite Sex on Show - Neville Greyling
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms4021.jpg" height="400" contain />
        Best Bird on Show and Best Champion on Show - Deon Davie
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms4022.jpg" height="400" contain />
        Best Intermediate on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms4023.jpg" height="400" contain />
        Best Novice on Show - Jacobs & Uys
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms4024.jpg" height="400" contain />
        Best Beginner on Show - Giel Calitz
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2002/ms4025.jpg" height="400" contain />
        Best Opposite Sex on Show - Nel Brothers Stud
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2002',
  data () {
    return {
      mini2019: [
        { date: '20 April 2002', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Intermediate' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Jacobs & Uys', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Giel Calitz', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '11 May 2002', award: 'Best Bird on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Sam Rosslee', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Molkentin Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Jacobs & Uys', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Kobus Hechter', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '24 August 2002', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Neville Greyling', status: 'Beginner' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: '.', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Neville Greyling', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '9 November', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Gert Pieters', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
