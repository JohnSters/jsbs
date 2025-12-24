<template>
  <div>
    <v-app-bar
      app
      color="deep-purple"
      dark
      fixed
    >
      <v-btn
        class="rounded-xl purple darken-4 hidden-md-and-up"
        text
        small
        @click="drawer = !drawer"
      >
        Main Menu
      </v-btn>
      <v-btn
        class="rounded-xl purple darken-4 hidden-sm-and-down"
        text
        @click="drawer = !drawer"
      >
        Main Menu
      </v-btn>
      <v-btn
        class="rounded-xl purple darken-3 ml-2 hidden-md-and-up"
        to="/society"
        text
        small
      >
        The Society
      </v-btn>
      <v-btn
        class="rounded-xl purple darken-3 ml-2 hidden-sm-and-down"
        to="/society"
        text
      >
        The Society
      </v-btn>
      <v-spacer />
      <v-btn
        class="mr-2 hidden-sm-and-down"
        href="https://www.showbudgies.co.za/shows/"
        target="_blank"
        color="purple darken-3"
        rounded
        small
        depressed
      >
        Upcoming Shows
      </v-btn>
      <v-btn
        class="mr-2 hidden-sm-and-down"
        href="https://www.showbudgies.co.za/results/results-main"
        target="_blank"
        color="purple darken-3"
        rounded
        small
        depressed
      >
        SA Show Results
      </v-btn>

      <v-bottom-sheet
        v-model="sheet"
      >
        <template #activator="{ on, attrs }">
          <v-btn
            class="mr-2"
            v-bind="attrs"
            icon
            small
            v-on="on"
          >
            <v-icon small>
              mdi-phone
            </v-icon>
          </v-btn>
        </template>
        <v-sheet
          class="text-center"
        >
          <v-btn
            class="mt-3 mb-3"
            text
            large
            color="error"
            @click="sheet = !sheet"
          >
            close
          </v-btn>
          <v-card>
            <v-simple-table>
              <template slot="default">
                <thead>
                  <tr>
                    <th class="text-left">
                      Society Members Name
                    </th>
                    <th class="text-left">
                      Office
                    </th>
                    <th class="text-left">
                      National Number
                    </th>
                  </tr>
                </thead>
                <tbody>
                  <tr
                    v-for="item in contacts"
                    :key="item.name"
                  >
                    <td class="text-left">
                      {{ item.name }}
                    </td>
                    <td class="text-left">
                      {{ item.office }}
                    </td>
                    <td class="text-left">
                      {{ item.number }}
                    </td>
                  </tr>
                </tbody>
              </template>
            </v-simple-table>
          </v-card>
        </v-sheet>
      </v-bottom-sheet>

      <v-btn class="mr-2" icon to="/" small>
        <v-icon small>
          mdi-home
        </v-icon>
      </v-btn>
    </v-app-bar>

    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <v-list
        class="mt-6"
        dense
        nav
      >
        <h3 class="blue-grey--text text-center">
          JSBS Navigation
        </h3>
        <v-divider class="ma-3" />
        <v-list-item-group
          v-for="(items, index) in menu"
          :key="index"
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item :to="items.src">
            <v-list-item-icon>
              <v-icon>{{ items.icon }}</v-icon>
            </v-list-item-icon>
            <v-list-item-title>{{ items.title }}</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  name: 'MainAppBar',
  data: () => ({
    sheet: false,
    drawer: null,
    group: null,
    contacts: [
      { name: 'Preggy Chetty', office: 'Chairman', number: '083 375 4776' },
      { name: 'Attie Van Staaden', office: 'Vice Chairman', number: '082 382 5925' },
      { name: 'Michael Borcherds', office: 'Treasurer', number: '082 441 7305' },
      { name: 'Todd Young', office: 'Secretary', number: '067 640 7504 ' },
      { name: 'Todd Young', office: 'Additional Member', number: '067-640-7504' }
    ],
    menu: [
      {
        title: 'Home',
        src: '/',
        icon: 'mdi-home'
      },
      {
        title: 'About Us',
        src: '/about',
        icon: 'mdi-account'
      },
      {
        title: 'Breeding',
        src: '/breeding',
        icon: 'mdi-trophy'
      },
      {
        title: 'Latest News',
        src: '/news',
        icon: 'mdi-note'
      },
      {
        title: 'JSBS Show Results',
        src: '/results',
        icon: 'mdi-podium'
      },
      {
        title: 'Club Champions',
        src: '/champions',
        icon: 'mdi-trophy'
      },
      {
        title: 'Show Budgie Hobby',
        src: '/hobby',
        icon: 'mdi-heart'
      },
      {
        title: 'Sales / Wanted',
        src: '/sales',
        icon: 'mdi-cash'
      }
    ]
  })
}
</script>

<style scoped>

</style>
