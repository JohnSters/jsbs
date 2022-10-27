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

        <v-row class="mt-6">
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1201.jpg"></v-img>
            <p class="text-center mt-2">Best Derby on Show and Best Derby Champion on Show - Nel Brothers Stud</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1202.jpg"></v-img>
            <p class="text-center mt-2">Best Derby Opposite Sex on Show and Best Derby Champion Opposite Sex on Show -
              Nel Brothers Stud</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1203.jpg"></v-img>
            <p class="text-center mt-2">Best Derby Novice on Show - Philip Jacobs</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1204.jpg"></v-img>
            <p class="text-center mt-2">Best Derby Novice Opposite Sex on Show - Rynier Burger</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1301.jpg"></v-img>
            <p class="text-center mt-2">Best Derby on Show and Best Derby Champion on Show - Nel Brothers Stud</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1302.jpg"></v-img>
            <p class="text-center mt-2">Best Derby Opposite Sex on Show and Best Derby Champion Opposite Sex on Show -
              Nel Brothers Stud</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1401.jpg"></v-img>
            <p class="text-center mt-2">Best Derby on Show JSBS and Best Derby Champion JSBS on Show and Best Derby
              Overall - Nel Brothers Stud</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1402.jpg"></v-img>
            <p class="text-center mt-2">Best Derby on Show JSBS and Best Derby Champion JSBS on Show - Nel Brothers
              Stud</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1403.jpg"></v-img>
            <p class="text-center mt-2">Best Derby Opposite Sex JSBS - Mike Davies.</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1501.jpg"></v-img>
            <p class="text-center mt-2">Best Derby on Show JSBS and Best Derby Champion JSBS on Show - Pierre Swart</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1502.jpg"></v-img>
            <p class="text-center mt-2">Best Derby Opposite Sex on Show JSBS and Best Derby Novice JSBS on Show - Cyril
              Nienaber</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1601.jpg"></v-img>
            <p class="text-center mt-2">Best Derby on Show JSBS and Best Derby Champion JSBS on Show - Pierre Swart</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1602.jpg"></v-img>
            <p class="text-center mt-2">Best Derby Opposite Sex on Show JSBS - Nel Brothers Stud</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1701.jpg"></v-img>
            <p class="text-center mt-2">Best Derby on Show JSBS and Best Derby Champion JSBS on Show - Pierre Swart</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1803.jpg"></v-img>
            <p class="text-center mt-2">Best Derby Bird on Show - Pierre Swart</p>
          </v-col>
          <v-col cols="12" sm="3">
            <v-img contain height="400" src="/images/budgies/derby/d1901.jpg"></v-img>
            <p class="text-center mt-2">Best Derby Resplendent Bird Aviaries.</p>
          </v-col>
        </v-row>

      </v-tab-item>

      <v-tab-item>

        <v-card class="pa-3">
          <v-row>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2023</p>
                <p>Show results coming soon</p>
                <v-btn block class="purple darken-1" depressed disabled rounded>Coming Soon</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2022</p>
                <p>Show results coming soon</p>
                <v-btn block class="purple darken-1" depressed disabled rounded>Coming Soon</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2021</p>
                <p>Cancelled due to Covid</p>
                <v-btn block class="purple darken-1" depressed disabled rounded>cancelled</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2020</p>
                <p>Cancelled due to Covid</p>
                <v-btn block class="purple darken-1" depressed disabled rounded>cancelled</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2019</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2019">View</v-btn>
              </v-card>
            </v-col>

            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2018</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2018">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2017</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2017">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2016</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2016">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2015</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2015">View</v-btn>
              </v-card>
            </v-col>

            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2014</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2014">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2013</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2013">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2012</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2012">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2011</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2011">View</v-btn>
              </v-card>
            </v-col>

            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2010</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2010">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2009</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2009">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2008</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2008">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2007</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2007">View</v-btn>
              </v-card>
            </v-col>

            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2006</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2006">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2005</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2005">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2004</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2004">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2003</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2003">View</v-btn>
              </v-card>
            </v-col>

            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2002</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2002">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2001</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2001">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 2000</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow2000">View</v-btn>
              </v-card>
            </v-col>
            <v-col cols="12" sm="3">
              <v-card class="pa-3 purple lighten-1 text-center" dark flat shaped>
                <p class="display-1 font-weight-light">Mini Show Results 1999</p>
                <v-btn block class="purple darken-1" depressed rounded to="/mini/MiniShow1999">View</v-btn>
              </v-card>
            </v-col>
          </v-row>
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
      {
        year: '2023',
        beginners: 'X',
        novice: '',
        intermediate: '',
        champion: '',
        opposite: '',
        show: 'Coming Soon'
      },
      {
        year: '2022',
        beginners: 'X',
        novice: '',
        intermediate: '',
        champion: '',
        opposite: '',
        show: 'Coming Soon'
      },
      {
        year: '2021',
        beginners: 'X',
        novice: '',
        intermediate: '',
        champion: '',
        opposite: '',
        show: 'Cancelled due to Covid'
      },
      {
        year: '2020',
        beginners: 'X',
        novice: '',
        intermediate: '',
        champion: '',
        opposite: '',
        show: 'Cancelled due to Covid'
      },
      {
        year: '2019',
        beginners: 'X',
        novice: 'The Grey Stud',
        intermediate: 'Retha van Deventer',
        champion: 'Resplendent Bird Aviaries',
        opposite: 'Nel Brothers Stud',
        show: 'Resplendent Bird Aviaries'
      },
      {
        year: '2018',
        beginners: 'X',
        novice: 'Grey Stud',
        intermediate: 'vd Heever Stud',
        champion: 'Pierre Swart',
        opposite: 'WW Aviaries',
        show: 'Pierre Swart'
      },
      {
        year: '2017',
        beginners: 'X',
        novice: 'No Entries',
        intermediate: 'vd Heever Stud',
        champion: 'Pierre Swart',
        opposite: 'Pierre Swart',
        show: 'Pierre Swart'
      },
      {
        year: '2016',
        beginners: 'X',
        novice: 'No Entries',
        intermediate: 'No Entries',
        champion: 'Pierre Swart',
        opposite: 'Nel Brothers Stud',
        show: 'Pierre Swart'
      },
      {
        year: '2015',
        beginners: 'X',
        novice: 'Cyril Nienaber',
        intermediate: 'No Entries',
        champion: 'Pierre Swart',
        opposite: 'Cyril Nienaber',
        show: 'Pierre Swart'
      },
      {
        year: '2014',
        beginners: 'X',
        novice: 'No Entries',
        intermediate: 'No Entries',
        champion: 'Nel Brothers Stud',
        opposite: 'Mike Davies',
        show: 'Nel Brothers Stud'
      },
      {
        year: '2013',
        beginners: 'X',
        novice: 'No Entries',
        intermediate: 'No Entries',
        champion: 'Nel Brothers Stud',
        opposite: 'Nel Brothers Stud',
        show: 'Nel Brothers Stud'
      },
      {
        year: '2012',
        beginners: 'X',
        novice: 'Philip Jacobs',
        intermediate: 'No Entries',
        champion: 'Nel Brothers Stud',
        opposite: 'Nel Brothers Stud',
        show: 'Nel Brothers Stud'
      },
      {
        year: '2011',
        beginners: 'X',
        novice: 'Rynier Burger',
        intermediate: 'No Entries',
        champion: 'Smartryk Burger',
        opposite: 'Rynier Burger',
        show: 'Smartryk Burger'
      },
      {
        year: '2010',
        beginners: 'X',
        novice: 'Clarence Marks',
        intermediate: 'No Entries',
        champion: 'Deon Davie',
        opposite: 'Deon Davies',
        show: 'Deon Davies'
      },
      {
        year: '2009',
        beginners: 'X',
        novice: 'Eric Wolmarans',
        intermediate: 'Gert Pieters',
        champion: 'Deon Davie',
        opposite: 'Deon Davies',
        show: 'Deon Davies'
      },
      {
        year: '2008',
        beginners: 'X',
        novice: 'Eric Wolmarans',
        intermediate: 'Gert Pieters',
        champion: 'Deon Davie',
        opposite: 'Nel Brothers Stud',
        show: 'Deon Davies'
      },
      {
        year: '2007',
        beginners: 'X',
        novice: 'Clarence Marks',
        intermediate: 'Gert Pieters',
        champion: 'Deon Davies',
        opposite: 'Gert Pieters',
        show: 'Deon Davies'
      },
      {
        year: '2006',
        beginners: 'X',
        novice: 'Clarence Marks',
        intermediate: 'Gert Pieters',
        champion: 'Nel Brothers Stud',
        opposite: 'Mike Davies',
        show: 'Clarence Marks'
      },
      {
        year: '2005',
        beginners: 'X',
        novice: 'Bill Sykes',
        intermediate: 'No Entries',
        champion: 'Pieter van der Linde',
        opposite: 'Deon Davie',
        show: 'Pieter van der Linde'
      },
      {
        year: '2004',
        beginners: 'X',
        novice: 'Neville Greyling',
        intermediate: 'Kobus Hechter',
        champion: 'Deon Davie',
        opposite: 'Nel Brothers Stud',
        show: 'Deon Davie'
      },
      {
        year: '2003',
        beginners: 'Neville Greyling',
        novice: '-',
        intermediate: 'Pieter van der Linde',
        champion: 'Nel Brothers Stud',
        opposite: 'Nel Brothers Stud',
        show: 'Nel Brothers Stud'
      },
      {
        year: '2002',
        beginners: '-',
        novice: '-',
        intermediate: '-',
        champion: '-',
        opposite: 'Sam Rosslee',
        show: 'Nel Brothers Stud'
      },
      {
        year: '2001',
        beginners: '-',
        novice: '-',
        intermediate: '-',
        champion: '-',
        opposite: 'Nel Brothers Stud',
        show: 'Molkentin Stud'
      },
      {
        year: '2000',
        beginners: '-',
        novice: '-',
        intermediate: '-',
        champion: '-',
        opposite: 'Nel Brothers Stud',
        show: 'Molkentin Stud'
      },
      {
        year: '1999',
        beginners: '-',
        novice: '-',
        intermediate: '-',
        champion: '-',
        opposite: '-',
        show: 'Nel Brothers Stud'
      }
    ]
  })
}
</script>

<style scoped>

</style>
