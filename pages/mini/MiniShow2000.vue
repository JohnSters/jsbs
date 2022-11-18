<template>
  <v-container>

    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1 mt-1" dark rounded text><v-icon class="mr-2">mdi-arrow-left</v-icon>Main Menu</v-btn>
      <v-btn to="/mini/MiniShow1999" class="purple darken-1 mt-1" dark rounded text>Mini Show 1999 <v-icon class="ml-2">mdi-arrow-right</v-icon></v-btn>
    </div>

    <h1>Mini Show Results 2000</h1>

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
      <v-col cols="12" sm="3">
        <v-img src="/images/budgies/minishow2000/bestb.jpg" height="400" contain></v-img>
        Best Bird on Show and Best Novice on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2000/bestos.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Andre Erasmus
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2000/interbbegos.jpg" height="400" contain></v-img>
        Best Champion on Show - Japie Smit
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2000/interbchos.jpg" height="400" contain></v-img>
        Best Intermediate on Show - Corrie van Staden
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2000/interbintos.jpg" height="400" contain></v-img>
        Best Beginner on Show - Jacobs and Uys
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2000/interbos.jpg" height="400" contain></v-img>
        Best Bird on Show - Molkentin Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2000/interbosos.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2000/molbb.jpg" height="400" contain></v-img>
        Best Bird on Show - Molkentin Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2000/nbsbos.jpg" height="400" contain></v-img>
        Best Opposite Sex on Show - Nel Brothers Stud
      </v-col>
    </v-row>

  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2000',
  data () {
    return {
      mini2019: [
        { date: '29 January 2000', award: 'Best Bird on Show', exh: 'Nel Brothers Stud', status: 'Novice' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Corrie van Staden', status: 'Intermediate' },
        { date: '.', award: 'Most Points on Show', exh: 'Nel Brothers Stud', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'Mike Davies', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Corrie van Staden', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Neville Greyling', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '26 February 2000', award: 'Best Bird on Show', exh: 'Japie Smit', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Novice' },
        { date: '.', award: 'Best Young Bird on Show', exh: 'Japie Smit', status: 'Champion' },
        { date: '.', award: 'Best Any Age on Show', exh: 'Japie Smit', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Japie Smit', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'CJ Bleasdale', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Neville Greyling', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '27 May 2000', award: 'Best Bird on Show', exh: 'Nel Brother Stud', status: 'Novice' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Andre Erasmus', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'Japie Smit', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Corrie van Staden', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Jacobs and Uys', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '29 July 2000', award: 'Best Bird on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'Molkentin Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Pieter van der Linde', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Neville Greyling', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '28 October 2000', award: 'Best Bird on Show', exh: 'Molkentin Stud', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Intermediate' },
        { date: '.', award: 'Best Champion on Show', exh: 'Molkentin Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Kobus Hechter', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
