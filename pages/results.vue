<template>
  <v-container>
    <v-card-title class="text-center justify-center py-6">
      <h1 class="font-weight-bold text-h2 basil--text">
        Show Results
      </h1>
    </v-card-title>

    <v-tabs
      v-model="tab"
      color="purple"
      grow
    >
      <v-tab>
        Derby Show Results
      </v-tab>
      <v-tab>
        Mini Show Results
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item>
        <v-card
          color="basil"
          flat
        >
          <v-card-text>
            <v-simple-table>
              <template v-slot:default>
                <thead>
                <tr>
                  <th class="text-left">
                    Derby Show
                  </th>
                  <th class="text-left">
                    Best Derby Beginners
                  </th>
                  <th class="text-left">
                    Best Derby Novice
                  </th>
                  <th class="text-left">
                    Best Derby Intermediate
                  </th>
                  <th class="text-left">
                    Best Derby Champion
                  </th>
                  <th class="text-left">
                    Best Derby Opposite Sex
                  </th>
                  <th class="text-left">
                    Best Derby on Show
                  </th>
                </tr>
                </thead>
                <tbody>
                <tr
                  v-for="item in derby"
                  :key="item.name"
                >
                  <td>{{ item.year }}</td>
                  <td>{{ item.beginners }}</td>
                  <td>{{ item.novice }}</td>
                  <td>{{ item.intermediate }}</td>
                  <td>{{ item.champion }}</td>
                  <td>{{ item.opposite }}</td>
                  <td>{{ item.show }}</td>
                </tr>
                </tbody>
              </template>
            </v-simple-table>
          </v-card-text>
        </v-card>
      </v-tab-item>

      <v-tab-item>
        <v-card
          color="basil"
          flat
        >
          <v-card-text>
              <v-row>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2023</p>
                    <v-btn class="purple darken-1" disabled rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2022</p>
                    <v-btn class="purple darken-1" disabled rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2021</p>
                    <v-btn class="purple darken-1" disabled rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2019</p>
                    <v-btn to="/mini/MiniShow2019" class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>

                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2018</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2017</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2016</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2015</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>

                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2014</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2013</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2012</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2011</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>

                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2010</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2009</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2008</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2007</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>

                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2006</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2005</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2004</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2003</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>

                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2002</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2001</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 2000</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
                <v-col cols="3" sm="3">
                  <v-card class="pa-3 purple lighten-1 text-center" flat dark shaped>
                    <p class="display-1 font-weight-light">Mini Show Results 1999</p>
                    <v-btn class="purple darken-1" rounded block depressed>View</v-btn>
                  </v-card>
                </v-col>
              </v-row>
          </v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-container>
</template>

<script>
export default {
  name: 'ShowResults',
  data: () => ({
    tab: null,
    derby: [
      { year: '2019', beginners: 'X', novice: 'The Grey Stud', intermediate: 'Retha van Deventer', champion: 'Resplendent Bird Aviaries', opposite: 'Nel Brothers Stud', show: 'Resplendent Bird Aviaries' },
      { year: '2018', beginners: 'X', novice: 'Grey Stud', intermediate: 'vd Heever Stud', champion: 'Pierre Swart', opposite: 'WW Aviaries', show: 'Pierre Swart' },
      { year: '2017', beginners: 'X', novice: 'No Entries', intermediate: 'vd Heever Stud', champion: 'Pierre Swart', opposite: 'Pierre Swart', show: 'Pierre Swart' },
      { year: '2016', beginners: 'X', novice: 'No Entries', intermediate: 'No Entries', champion: 'Pierre Swart', opposite: 'Nel Brothers Stud', show: 'Pierre Swart' },
      { year: '2015', beginners: 'X', novice: 'Cyril Nienaber', intermediate: 'No Entries', champion: 'Pierre Swart', opposite: 'Cyril Nienaber', show: 'Pierre Swart' },
      { year: '2014', beginners: 'X', novice: 'No Entries', intermediate: 'No Entries', champion: 'Nel Brothers Stud', opposite: 'Mike Davies', show: 'Nel Brothers Stud' },
      { year: '2013', beginners: 'X', novice: 'No Entries', intermediate: 'No Entries', champion: 'Nel Brothers Stud', opposite: 'Nel Brothers Stud', show: 'Nel Brothers Stud' },
      { year: '2012', beginners: 'X', novice: 'Philip Jacobs', intermediate: 'No Entries', champion: 'Nel Brothers Stud', opposite: 'Nel Brothers Stud', show: 'Nel Brothers Stud' },
      { year: '2011', beginners: 'X', novice: 'Rynier Burger', intermediate: 'No Entries', champion: 'Smartryk Burger', opposite: 'Rynier Burger', show: 'Smartryk Burger' },
      { year: '2010', beginners: 'X', novice: 'Clarence Marks', intermediate: 'No Entries', champion: 'Deon Davie', opposite: 'Deon Davies', show: 'Deon Davies' },
      { year: '2009', beginners: 'X', novice: 'Eric Wolmarans', intermediate: 'Gert Pieters', champion: 'Deon Davie', opposite: 'Deon Davies', show: 'Deon Davies' },
      { year: '2008', beginners: 'X', novice: 'Eric Wolmarans', intermediate: 'Gert Pieters', champion: 'Deon Davie', opposite: 'Nel Brothers Stud', show: 'Deon Davies' },
      { year: '2007', beginners: 'X', novice: 'Clarence Marks', intermediate: 'Gert Pieters', champion: 'Deon Davies', opposite: 'Gert Pieters', show: 'Deon Davies' },
      { year: '2006', beginners: 'X', novice: 'Clarence Marks', intermediate: 'Gert Pieters', champion: 'Nel Brothers Stud', opposite: 'Mike Davies', show: 'Clarence Marks' },
      { year: '2005', beginners: 'X', novice: 'Bill Sykes', intermediate: 'No Entries', champion: 'Pieter van der Linde', opposite: 'Deon Davie', show: 'Pieter van der Linde' },
      { year: '2004', beginners: 'X', novice: 'Neville Greyling', intermediate: 'Kobus Hechter', champion: 'Deon Davie', opposite: 'Nel Brothers Stud', show: 'Deon Davie' },
      { year: '2003', beginners: 'Neville Greyling', novice: '-', intermediate: 'Pieter van der Linde', champion: 'Nel Brothers Stud', opposite: 'Nel Brothers Stud', show: 'Nel Brothers Stud' },
      { year: '2002', beginners: '-', novice: '-', intermediate: '-', champion: '-', opposite: 'Sam Rosslee', show: 'Nel Brothers Stud' },
      { year: '2001', beginners: '-', novice: '-', intermediate: '-', champion: '-', opposite: 'Nel Brothers Stud', show: 'Molkentin Stud' },
      { year: '2000', beginners: '-', novice: '-', intermediate: '-', champion: '-', opposite: 'Nel Brothers Stud', show: 'Molkentin Stud' },
      { year: '1999', beginners: '-', novice: '-', intermediate: '-', champion: '-', opposite: '-', show: 'Nel Brothers Stud' }
    ]
  })
}
</script>

<style scoped>

</style>
