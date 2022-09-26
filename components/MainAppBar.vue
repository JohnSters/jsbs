<template>
  <div>
    <v-app-bar
      app
      color="deep-purple"
      dark
      fixed
    >
      <v-btn class="rounded-xl purple darken-4" @click="drawer = !drawer">Main Menu</v-btn>
      <v-spacer></v-spacer>
      <v-btn
        class="mr-2"
        href="https://www.showbudgies.co.za/shows/"
        rounded
        small
        target="_blank"
        text
      >
        Shows
      </v-btn>
      <v-btn
        class="mr-2"
        href="https://www.showbudgies.co.za/results/results-main"
        rounded
        small
        target="_blank"
        text
      >
        Results
      </v-btn>
      <v-btn class="mr-3" icon to="/">
        <v-icon>mdi-phone</v-icon>
      </v-btn>
      <v-btn class="mr-3" icon to="/">
        <v-icon>mdi-home</v-icon>
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
        <h3 class="blue-grey--text text-center">JSBS Navigation</h3>
        <v-divider class="ma-3"></v-divider>
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
    drawer: null,
    group: null,
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
        title: 'Latest News',
        src: '/news',
        icon: 'mdi-note'
      },
      {
        title: 'The Society',
        src: '/society',
        icon: 'mdi-account-group'
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
