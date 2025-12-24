<template>
  <v-container>
    <div class="text-center mb-6">
      <v-btn to="/results" class="purple darken-1" dark rounded text>
        <v-icon class="mr-2">
          mdi-arrow-left
        </v-icon>Main Menu
      </v-btn>
      <v-btn to="/mini/MiniShow2003" class="purple darken-1" dark rounded text>
        Mini Show 2003 <v-icon class="ml-2">
          mdi-arrow-right
        </v-icon>
      </v-btn>
    </div>

    <h1>Mini Show Results 2004</h1>

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
  </v-container>
</template>

<script>
export default {
  name: 'MiniShow2004',
  data () {
    return {
      mini2019: [
        { date: '31 January 2004', award: 'Best Bird on Show', exh: 'Sam Rosslee', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Bill Sykes', status: 'Novice' },
        { date: '.', award: 'Best Champion on Show', exh: 'Sam Rosslee', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Kobus Hechter', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Bill Sykes', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '15 May 2004', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Kobus Hechter', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Wim Vrey', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '19 June 2004', award: 'Best Bird on Show', exh: 'Daan Coetzee', status: 'Novice' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Sam Rosslee', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Corrie van Staden', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Daan Coetzee', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '17 July 2004', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'No Entries', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Wim Vrey', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '28 August 2004', award: 'Best Bird on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Deon Davie', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Clarence Marks', status: '.' },
        { date: '', award: '', exh: '', status: '' },

        { date: '9 October 2004', award: 'Best Bird on Show', exh: 'Pieter van der Linde', status: 'Champion' },
        { date: '.', award: 'Best Opposite Sex on Show', exh: 'Deon Davie', status: 'Champion' },
        { date: '.', award: 'Best Champion on Show', exh: 'Pieter van der Linde', status: '.' },
        { date: '.', award: 'Best Intermediate on Show', exh: 'Gert Pieters', status: '.' },
        { date: '.', award: 'Best Novice on Show', exh: 'Daan Coetzee', status: '.' }
      ]
    }
  }
}
</script>

<style scoped>

</style>
