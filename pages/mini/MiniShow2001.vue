<template>
  <v-container>
    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text>
        <v-icon class="mr-2">
          mdi-arrow-left
        </v-icon>Main Menu
      </v-btn>
      <v-btn to="/mini/MiniShow2000" class="purple darken-1" dark rounded text>
        Mini Show 2000 <v-icon class="ml-2">
          mdi-arrow-right
        </v-icon>
      </v-btn>
    </div>

    <h1>Mini Show Results 2001</h1>

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
        <v-img src="/images/budgies/minishow2001/ms011.jpg" height="400" contain />
        Best Beginner on Show - Kobus Hechter
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2001/ms012.jpg" height="400" contain />
        Best Bird and Best Intermediate on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2001/ms1011.jpg" height="400" contain />
        Best Bird on Show and Best Intermediate - Corrie van Staden
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2001/ms1012.jpg" height="400" contain />
        Best Beginner on Show - Kobus Hechter
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2001/ms1013.jpg" height="400" contain />
        Best Champion on Show - Molkentin Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2001/ms1014.jpg" height="400" contain />
        Best Bird on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2001/ms1015.jpg" height="400" contain />
        Second Best on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2001/ms4011.jpg" height="400" contain />
        Best Opposite Sex on Show - Nel Brothers Stud
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2001/ms4012.jpg" height="400" contain />
        Best Champion on Show - Sam Rosslee
      </v-col>
      <v-col cols="2">
        <v-img src="/images/budgies/minishow2001/ms4015.jpg" height="400" contain />
        Best Beginner on Show - Jacobs & Uys
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2001',
  data () {
    return {
      mini2019: [
        { date: '27 January 2001', award: 'Best Bird on Show', exh: 'Nel Brothers Stud', status: 'Intermediate' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Intermediate' },
        { date: '.', award: 'Best Champion on Show', exh: 'No entries', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Novices in club', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Kobus Hechter', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '28 April 2001', award: 'Best Bird on Show', exh: 'Corrie van Staden', status: 'Intermediate' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Jacobs & Uys', status: 'Beginner' },
        { date: '.', award: 'Best Champion on Show', exh: 'Molkentin Stud', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Corrie van Staden', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Novices in club', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Kobus Hechter', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '21 July 2001', award: 'Best Bird on Show', exh: 'Corrie van Staden', status: 'Intermediate' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Kevin Weinmann', status: 'Beginner' },
        { date: '.', award: 'Best Champion on Show', exh: 'Mike Davies', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Corrie van Staden', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Novices in club', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Kobus Hechter', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '27 October 2001', award: 'Best Bird on Show', exh: 'Nel Brothers Stud', status: 'Intermediate' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Nel Brothers Stud', status: 'Intermediate' },
        { date: '.', award: 'Best Champion on Show', exh: 'Sam Rosslee', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Nel Brothers Stud', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'No Novices in club', status: '.' },
        { date: '.', award: 'Best Beginner on Show', exh: 'Jacobs & Uys', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
