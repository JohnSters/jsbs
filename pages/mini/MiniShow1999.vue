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
      <v-col cols="12" sm="4">
        <v-img src="/images/budgies/minishow1999/bb.jpg" height="400" contain></v-img>
      </v-col>
      <v-col cols="12" sm="4">
        <v-img src="/images/budgies/minishow1999/bb910.jpg" height="400" contain></v-img>
      </v-col>
      <v-col cols="12" sm="4">
        <v-img src="/images/budgies/minishow1999/bos.jpg" height="400" contain></v-img>
      </v-col>
    </v-row>

  </v-container>
</template>

<script>
export default {
  name: 'MiniShow1999',
  data () {
    return {
      mini2019: [
        { date: '16 January 1999', award: 'Best Bird on Show', exh: 'Corrie van Staden', status: 'Intermediate' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Neville Greyling', status: 'Beginner' },
        { date: '.', award: 'Most Points on Show', exh: 'Nel Brothers Stud', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Corrie van Staden', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Neville Greyling', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '24 April 1999', award: 'Best Bird on Show', exh: 'Japie Smit', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Corrie van Staden', status: 'Intermediate' },
        { date: '.', award: 'Most Points on Show', exh: 'Japie Smit', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Japie Smit', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Corrie van Staden', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Neville Greyling', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '14 August 1999', award: 'Best Bird on Show', exh: 'Mike Davies', status: 'Intermediate' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Novice' },
        { date: '.', award: 'Most Points on Show', exh: 'Nel Brothers Stud', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Mike Davies', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Neville Greyling', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '9 October 1999', award: 'Best Bird on Show', exh: 'Nel Brothers Stud', status: 'Novice' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Novice' },
        { date: '.', award: 'Most Points on Show', exh: 'Nel Brothers Stud', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'Mike Davies', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Corrie van Staden', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'M & G Stud', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
