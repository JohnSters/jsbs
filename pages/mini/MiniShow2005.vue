<template>
  <v-container>

    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text><v-icon class="mr-2">mdi-arrow-left</v-icon>Main Menu</v-btn>
      <v-btn to="/mini/MiniShow2004" class="purple darken-1" dark rounded text>Mini Show 2004 <v-icon class="ml-2">mdi-arrow-right</v-icon></v-btn>
    </div>

    <h1>Mini Show Results 2005</h1>

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
        <v-img src="/images/budgies/minishow2005/ms1053.jpg" height="400" contain></v-img>
        Best Bird on Show - Molkentin Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms1054.jpg" height="400" contain></v-img>
        Best Novice on Show - Bill Sykes
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms1055.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Molkentin Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms2053.jpg" height="400" contain></v-img>
        Best Bird on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms3054.jpg" height="400" contain></v-img>
        Best Bird on Show - Deon Davie
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms3055.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show and Best Novice on Show - Bill Sykes
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms3056.jpg" height="400" contain></v-img>
        Best Champion Opposite Sex on Show - Deon Davie
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms3057.jpg" height="400" contain></v-img>
        Best Intermediate on Show - Gert Pieters
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms4051.jpg" height="400" contain></v-img>
        Best Bird on Show - Deon Davie
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms4052.jpg" height="400" contain></v-img>
        Best Intermediate on Show - Gert Pieters
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms4053.jpg" height="400" contain></v-img>
        Best Novice on Show - Bill Sykes
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2005/ms4054.jpg" height="400" contain></v-img>
        Best Opposite sex on Show - Deon Davie
      </v-col>
    </v-row>

  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2005',
  data () {
    return {
      mini2019: [
        { date: '2 April 2005', award: 'Best Bird on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Molkentin Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Bill Sykes', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '7 May 2005', award: 'Best Bird on Show', exh: 'Nel Brothers Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Bill Sykes', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '25 June 2005', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Bill Sykes', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Bill Sykes', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '27 August 2005', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Bill Sykes', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '8 October 2005', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Bill Sykes', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
