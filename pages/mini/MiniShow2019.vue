<template>
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
        <td>{{ item.name }}</td>
        <td>{{ item.calories }}</td>
      </tr>
      </tbody>
    </template>
  </v-simple-table>
</template>

<script>
export default {
  name: 'MiniShow2019',
  data () {
    return {
      mini2019: [
        {
          name: 'Frozen Yogurt',
          calories: 159
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
