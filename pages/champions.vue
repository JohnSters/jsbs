<template>
  <v-container>
    <v-row>
      <v-col cols="12" sm="6" v-for="(item, id) in items" :key="id">
        <v-card class="pa-3" shaped>
          <v-card width="300" class="ma-auto rounded-0 pa-2 purple lighten-5">
            <v-img :src="item.img" height="300" contain></v-img>
          </v-card>
          <p class="mt-3 purple text-center darken-3 pa-1 rounded-xl white--text"><v-icon class="mr-3" dark>mdi-trophy</v-icon>{{ item.title }}</p>
          <b>{{ item.results }}</b>
          <ul>
            <li>{{ item.results_a }} <br> <b>{{ item.result_points_a }}</b></li>
            <li>{{ item.results_b }} <br> <b>{{ item.result_points_b }}</b></li>
            <li>{{ item.results_c }} <br> <b>{{ item.result_points_c }}</b></li>
          </ul>
          <hr class="ma-3 purple lighten-4">
          <b>{{  item.shows }}</b>
          <ul>
            <li>{{ item.shows_a }} <br> <b>{{ item.shows_points_a }}</b></li>
            <li>{{ item.shows_b }} <br> <b>{{ item.shows_points_b }}</b></li>
            <li>{{ item.shows_c }} <br> <b>{{ item.shows_points_c }}</b></li>
          </ul>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'ChampionsPage',
  data: () => ({
    items: [
      {
        title: 'Club Champion 2019 - Pierre Swart',
        img: '/images/champions/ps2017.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions ',
        result_points_a: '- Pierre Swart (21 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Retha van Deventer (10 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- The Grey Stud (8 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Resplendent Bird Aviaries (491 points)',
        shows_b: 'Most Points - Intermediate',
        shows_points_b: '- vd Heever Stud (268 points)',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Henk Potgieter (298 points)'
      },
      {
        title: 'Club Champion 2018 - Pierre Swart',
        img: '/images/champions/ps2017.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Pierre Swart (15 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- None',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- None',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Resplendent Bird Aviaries (367 points)',
        shows_b: 'Most Points',
        shows_points_b: '- None',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- None'
      },
      {
        title: 'Club Champion 2017 - Pierre Swart',
        img: '/images/champions/ps2017.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Pierre Swart (16 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Rynier Burger (12 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Bill Stanley (8 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud (232 points)',
        shows_b: 'Most Points',
        shows_points_b: '- Rynier Burger (368 points)',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Bill Stanley (55 points)'
      },
      {
        title: 'Club Champion 2016 - Ryan van der Heever ',
        img: '/images/champions/rvdh.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Mike Davies (21 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Rynier Burger (17 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Ryan van der Heever (25 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud (295 points)',
        shows_b: 'Most Points',
        shows_points_b: '- Rynier Burger (95 points)',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Ryan van der Heever (227 points)'
      },
      {
        title: 'Club Champion 2015 - John and Ian Nel, Nel Brothers Stud ',
        img: '/images/champions/nbs1.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Nel Brothers Stud (45 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- None',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Bill Stanley (22 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Nel Brothers Stud (44 points)',
        shows_b: 'Most Points',
        shows_points_b: '- None',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- None'
      },
      {
        title: 'Club Champion 2014 - John and Ian Nel, Nel Brothers Stud ',
        img: '/images/champions/nbs1.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Nel Brothers Stud (28 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- None',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- None',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Nel Brothers Stud (34 points)',
        shows_b: 'Most Points',
        shows_points_b: '- None',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- None'
      },
      {
        title: 'Club Champion 2013 - John and Ian Nel, Nel Brothers Stud ',
        img: '/images/champions/nbs1.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Nel Brothers Stud (34 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- None',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Koos du Preez (27 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Nel Brothers Stud (67 points)',
        shows_b: 'Most Points',
        shows_points_b: '- None',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Koos du Preez (106 points)'
      },
      {
        title: 'Club Champion 2012 - Rynier Burger',
        img: '/images/champions/rb.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Nel Brothers Stud (64 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Gert Pieters (66 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Rynier Burger (107 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Nel Brothers Stud with 36',
        shows_b: 'Most Points',
        shows_points_b: '- Gert Pieters with 54',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Rynier Burger with 68'
      },
      {
        title: 'Club Champion 2011 - Clarence Marks',
        img: '/images/champions/',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Nel Brothers Stud (58 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Gert Pieters (55 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Clarence Marks (68 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Smartryk Burger with 35',
        shows_b: 'Most Points',
        shows_points_b: '- Gert Pieters with 78',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Rynier Burger with 36'
      },
      {
        title: 'Club Champion 2010 - Gert Pieters',
        img: '/images/champions/gp06.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Smartryk Burger (29 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Gert Pieters (65 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Grobbelaar Stud (32 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud with 319',
        shows_b: 'Most Points',
        shows_points_b: '- Eric Wolmarans with 117',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Grobbelaar Stud with 72'
      },
      {
        title: 'Club Champion 2009 - Gert Pieters',
        img: '/images/champions/gp06.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Deon Davie (98 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Gert Pieters (115 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Clarence Marks (53 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud with 120',
        shows_b: 'Most Points',
        shows_points_b: '- Gert Pieters with 70',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Clarence Marks with 64'
      },
      {
        title: 'Club Champion 2008 - Mike Davies',
        img: '/images/champions/jsbs2008.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Mike Davies (46 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Gert Pieters (43 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Clarence Marks (25 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud with 390',
        shows_b: 'Most Points',
        shows_points_b: '- Gert Pieters with 54',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- APJ Swanepoel with 121'
      },
      {
        title: 'Club Champion 2007 - Gert Pieters',
        img: '/images/champions/gp06.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Nel Brothers Stud (55 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Gert Pieters (74 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Clarence Marks (49 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud with 250',
        shows_b: 'Most Points',
        shows_points_b: '- Gert Pieters with 30',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Clarence Marks with 27'
      },
      {
        title: 'Club Champion 2006 - Gert Pieters',
        img: '/images/champions/gp06.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Nel Brothers Stud (78 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Gert Pieters (147 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Bill Sykes (67 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud with 368',
        shows_b: 'Most Points',
        shows_points_b: '- Gert Pieters with 39',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Bill Sykes with 78'
      },
      {
        title: 'Club Champion 2005 - Bill Sykes',
        img: '/images/champions/bs.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Deon Davie (123 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Gert Pieters (115 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Bill Sykes (129 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud with 237',
        shows_b: 'Most Points',
        shows_points_b: '- Gert Pieters with 17',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Bill Sykes with 48'
      },
      {
        title: 'Club Champion 2004 - Deon Davie',
        img: '/images/champions/dd.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Deon Davie (133 points)',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Gert Pieters (56 points)',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Daan Coetzee (100 points)',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud with 310',
        shows_b: 'Most Points',
        shows_points_b: '- Kobus Hechter with 24',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Bill Sykes with 15'
      },
      {
        title: 'Club Champion 2003 - Gert Pieters',
        img: '/images/champions/gp.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Deon Davie',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Pieter van der Linde',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- None',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud with 147',
        shows_b: 'Most Points',
        shows_points_b: '- None',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- None'
      },
      {
        title: 'Club Champion 2002 - Gert Pieters',
        img: '/images/champions/gp.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Deon Davie',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Nel Brothers Stud',
        results_c: 'JSBS Champion of Novices',
        result_points_c: '- Jacobs&Uys',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud with 412',
        shows_b: 'Most Points - Intermediate',
        shows_points_b: '- Nel Brothers Stud with 193',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- ISW Smit with 83'
      },
      {
        title: 'Club Champion 2001 - The Nel Brothers Stud, John and Ian Nel',
        img: '/images/champions/nbs1.jpg',
        results: 'The results were as follow:',
        results_a: 'JSBS Champion of Champions',
        result_points_a: '- Nel Brothers Stud',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: '- Nel Brothers Stud',
        results_c: 'JSBS Champion of Beginners',
        result_points_c: '- Kobus Hechte',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: '- Molkentin Stud with 360',
        shows_b: 'Most Points - Intermediate',
        shows_points_b: '- Nel Brothers Stud with 176',
        shows_c: 'Most Points - Novice',
        shows_points_c: '- Russell Dixon with 67'
      },
      {
        title: 'Club Champion 2000 - The Nel Brothers Stud, John and Ian Nel',
        img: '/images/champions/nbs.jpg',
        results: 'The results were as follow:',
        result_points_a: 'Nel Brothers Stud - 100',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: 'Molkentin Stud - 67',
        results_c: 'JSBS Champion of Beginners',
        result_points_c: 'Corrie van Staden - 35',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: 'None',
        shows_b: 'Most Points - Intermediate',
        shows_points_b: 'None',
        shows_c: 'Most Points - Novice',
        shows_points_c: 'None'
      },
      {
        title: 'Club Champion 1999 - The Nel Brothers Stud, John and Ian Nel',
        img: '/images/champions/nbs.jpg',
        results: 'The results were as follow:',
        result_points_a: 'Nel Brothers Stud - 139',
        results_b: 'JSBS Champion of Intermediates',
        result_points_b: 'Mike Davies - 87',
        results_c: 'JSBS Champion of Beginners',
        result_points_c: 'Neville Greyling - 80',
        shows: 'The results for most points at Championship Shows were as follows:',
        shows_a: 'Most Points - Champion',
        shows_points_a: 'None',
        shows_b: 'Most Points - Intermediate',
        shows_points_b: 'None',
        shows_c: 'Most Points - Novice',
        shows_points_c: 'None'
      }
    ]
  })
}
</script>

<style scoped>

</style>
