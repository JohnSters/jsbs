<template>
  <v-container>

    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text><v-icon class="mr-2">mdi-arrow-left</v-icon>Main Menu</v-btn>
      <v-btn to="/mini/MiniShow2002" class="purple darken-1" dark rounded text>Mini Show 2002 <v-icon class="ml-2">mdi-arrow-right</v-icon></v-btn>
    </div>

    <h1>Mini Show Results 2003</h1>

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
        <v-img src="/images/budgies/minishow2003/ms1031.jpg" height="400" contain></v-img>
        Best Opposite Sex in Show - Corrie van Staden
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms1032.jpg" height="400" contain></v-img>
        Best Intermediate in Show - Pieter van der Linde
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms1033.jpg" height="400" contain></v-img>
        Best Beginner in Show - Neville Greyling
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms2031.jpg" height="400" contain></v-img>
        Best Bird on Show - Molkentin Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms2032.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Corrie van Staden
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms3031.jpg" height="400" contain></v-img>
        Best Bird on Show - Deon Davie
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms3032.jpg" height="400" contain></v-img>
        Best Intermediate on Show - Pieter van der Linde
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms3033.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Gert Pieters
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms4031.jpg" height="400" contain></v-img>
        Best Bird on Show - Gert Pieters
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms4032.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Deon Davie
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms4033.jpg" height="400" contain></v-img>
        Best Intermediate on Show - Pieter van der Linde
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms5031.jpg" height="400" contain></v-img>
        Best Opposite Sex Champion on Show - Deon Davie
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms6032.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Sam Rosslee
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2003/ms6033.jpg" height="400" contain></v-img>
        Best Beginner on Show - Daan Coetzee
      </v-col>
    </v-row>

  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2003',
  data () {
    return {
      mini2019: [
        { date: '1 February 2003', award: 'Best Bird on Show', exh: 'Nel Brothers Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Corrie van Staden', status: 'Intermediate' },
        { date: '.', award: 'Best Champion on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Pieter van der Linde', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Neville Greyling', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '12 April 2003', award: 'Best Bird on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Molkentin Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Pieter van der Linde', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Gert Pieters', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '17 May 2003', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Gert Pieters', status: 'Beginner' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Pieter van der Linde', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Gert Pieters', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '30 August 2003', award: 'Best Bird on Show', exh: 'Gert Pieters', status: 'Beginner' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Pieter van der Linde', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Gert Pieters', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '11 October 2003', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Gert Pieters', status: 'Beginner' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Corrie van Staden', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Daan Coetzee', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '1 November 2003', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Sam Rosslee', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Gert Pieters', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
