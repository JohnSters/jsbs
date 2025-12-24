<template>
  <v-container fluid>
    <v-card-title class="text-center justify-center py-6 hidden-md-and-up">
      <h3 class="font-weight-bold basil--text">
        Budgerigar Breeding
      </h3>
    </v-card-title>

    <v-card-title class="text-center justify-center py-6 hidden-sm-and-down">
      <h3 class="font-weight-bold text-h2 basil--text">
        Budgerigar Breeding
      </h3>
    </v-card-title>

    <v-toolbar color="grey" class="mt-3" flat>
      <h3 class="white--text">
        Albino
      </h3>
    </v-toolbar>

    <v-simple-table dense>
      <template #default>
        <thead>
          <tr>
            <th class="text-left" style="width: 40%">
              Pairing
            </th>
            <th class="text-left">
              Expectation
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Albino x Albino</td>
            <td>
              <ul>
                <li>100% Albino</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Albino Cock x Normal Hen</td>
            <td>
              <ul>
                <li>Normal/Albino Cocks</li>
                <li>Albino Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Albino Cocks x Albino Hens</td>
            <td>
              <ul>
                <li>Albino Cocks</li>
                <li>Normal/Albino Cocks</li>
                <li>Albino Hens</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal Cock x Albino Hen</td>
            <td>
              <ul>
                <li>Normal/Albino Cocks</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Albino Cock x Normal Hen</td>
            <td>
              <ul>
                <li>Normal Cocks</li>
                <li>Normal/Albino Cocks</li>
                <li>Albino Hens</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-toolbar color="#D2691E" class="mt-3" flat>
      <h3 class="white--text">
        Cinnamon
      </h3>
    </v-toolbar>

    <v-simple-table dense>
      <template #default>
        <thead>
          <tr>
            <th class="text-left" style="width: 40%">
              Pairing
            </th>
            <th class="text-left">
              Expectation
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Cinnamon Cock x Cinnamon Hen</td>
            <td>
              <ul>
                <li>100% Cinnamon</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Cinnamon Cock x Normal Hen</td>
            <td>
              <ul>
                <li>Normal/Cinnamon Cocks</li>
                <li>Cinnamon Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Cinnamon Cock x Cinnamon Hen</td>
            <td>
              <ul>
                <li>Cinnamon Cocks</li>
                <li>Normal/Cinnamon Cocks</li>
                <li>Cinnamon Hens</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Cinnamon Cock x Normal Hen</td>
            <td>
              <ul>
                <li>Normal/Cinnamon Cocks</li>
                <li>Normal Cocks</li>
                <li>Cinnamon Hens</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal Cock x Cinnamon Hen</td>
            <td>
              <ul>
                <li>Normal/Cinnamon Cocks</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-toolbar color="blue-grey" class="mt-3" flat>
      <h3 class="white--text">
        Dark-Eyed Clear
      </h3>
    </v-toolbar>

    <v-simple-table dense>
      <template #default>
        <thead>
          <tr>
            <th class="text-left" style="width: 40%">
              Pairing
            </th>
            <th class="text-left">
              Expectation
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Clearflight(DF) x Recessive Pied</td>
            <td>
              <ul>
                <li>50% Clearflighted/Rec Pied</li>
                <li>50% Normal/Rec Pied</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Clearflighted (SF)/Rec Pied x Rec Pied</td>
            <td>
              <ul>
                <li>25% Recessive Pied</li>
                <li>25% Normal/Rec Pied</li>
                <li>25% Clearflighted(SF)/Rec Pied</li>
                <li>25% Dark-Eyed Clear</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Clearflighted(DF) x Rec Pied</td>
            <td>
              <ul>
                <li>100% Clearflighted(SF)/Rec Pied</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Dark-Eyed Clear x Rec Pied</td>
            <td>
              <ul>
                <li>50% Dark-Eyed Clear</li>
                <li>50% Rec Pied</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Dark-Eyed Clear(SF) x Dark-Eyed Clear(SF)</td>
            <td>
              <ul>
                <li>50% Dark-Eyed Clear(SF)</li>
                <li>25% Dark-Eyed Clear(DF)</li>
                <li>25% Rec Pied</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Dark-Eyed Clear(SF) x Clearflighted(SF)</td>
            <td>
              <ul>
                <li>50% Clearflighted(DF)/Rec Pied</li>
                <li>50% Clearflighted(SF)/Rec Pied</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Dark-Eyed Clear(SF) x Clearflighted(DF)/Rec Pied</td>
            <td>
              <ul>
                <li>25% Dark-Eyed Clear(SF)</li>
                <li>25% Dark-Eyed Clear(DF)</li>
                <li>25% Clearflighted(SF)/Rec Pied</li>
                <li>25% Clearflighted(DF)/Rec Pied</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Dark-Eyed Clear(SF) x Clearflighted(SF)/Rec Pied</td>
            <td>
              <ul>
                <li>12,5% Dark-Eyed Clear(DF)</li>
                <li>25% Dark-Eyed Clear(SF)</li>
                <li>12,5% Rec Pied</li>
                <li>12,5% Clearflighted(DF)/Rec Pied</li>
                <li>25% Clearflighted(SF)/Rec Pied</li>
                <li>12,5% Normal/Rec Pied</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-toolbar color="purple darken-3" class="mt-3" flat>
      <h3 class="white--text">
        Dominant Pied
      </h3>
    </v-toolbar>

    <v-simple-table dense>
      <template #default>
        <thead>
          <tr>
            <th class="text-left" style="width: 40%">
              Pairing
            </th>
            <th class="text-left">
              Expectation
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Dominant Pied(SF) x Normal</td>
            <td>
              <ul>
                <li>50% Dominant Pied(SF)</li>
                <li>50% Normal</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Dominant Pied(DF) x Normal</td>
            <td>
              <ul>
                <li>100% Dominant Pied(SF)</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Dominant Pied(SF) x Dominant Pied(SF)</td>
            <td>
              <ul>
                <li>25% Normal</li>
                <li>50% Dominant Pied(SF)</li>
                <li>25% Dominant Pied(DF)</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Dominant Pied(SF) x Dominant Pied(DF)</td>
            <td>
              <ul>
                <li>50% Dominant Pied(SF)</li>
                <li>50% Dominant Pied(DF)</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Dominant Pied(DF) x Dominant Pied(DF)</td>
            <td>
              <ul>
                <li>100% Dominant Pied(DF)</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-toolbar color="purple darken-1" class="mt-3" flat>
      <h3 class="white--text">
        Fallow
      </h3>
    </v-toolbar>

    <v-simple-table dense>
      <template #default>
        <thead>
          <tr>
            <th class="text-left" style="width: 40%">
              Pairing
            </th>
            <th class="text-left">
              Expectation
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Normal x Normal/Fallow</td>
            <td>
              <ul>
                <li>50% Normal</li>
                <li>50% Normal/Fallow</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal x Fallow</td>
            <td>
              <ul>
                <li>100% Normal/Fallow</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Fallow x Normal/Fallow</td>
            <td>
              <ul>
                <li>25% Normal</li>
                <li>50% Normal/Fallow</li>
                <li>25% Fallow</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Fallow x Normal/Fallow</td>
            <td>
              <ul>
                <li>25% Normal</li>
                <li>50% Normal/Fallow</li>
                <li>25% Fallow</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Fallow x Fallow</td>
            <td>
              <ul>
                <li>50% Normal/Fallow</li>
                <li>50% Fallow</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Fallow x Fallow</td>
            <td>
              <ul>
                <li>100% Fallow</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-toolbar color="yellow darken-2" class="mt-3" flat>
      <h3 class="white--text">
        Lutino
      </h3>
    </v-toolbar>

    <v-simple-table dense>
      <template #default>
        <thead>
          <tr>
            <th class="text-left" style="width: 40%">
              Pairing
            </th>
            <th class="text-left">
              Expectation
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Lutino x Lutino</td>
            <td>
              <ul>
                <li>100% Lutino</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Lutino Cock x Normal Hen</td>
            <td>
              <ul>
                <li>Normal/Lutino Cocks</li>
                <li>Lutino Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Lutino Cock x Lutino Hen</td>
            <td>
              <ul>
                <li>Lutino Cocks</li>
                <li>Normal/Lutino Cocks</li>
                <li>Lutino Hens</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Lutino Cock x Lutino Hen</td>
            <td>
              <ul>
                <li>Normal/Lutino Cocks</li>
                <li>Normal Cocks</li>
                <li>Lutino Hens</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal Cock x Lutino Hen</td>
            <td>
              <ul>
                <li>Normal/Lutino Cocks</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-toolbar color="blue darken-2" class="mt-3" flat>
      <h3 class="white--text">
        Opaline
      </h3>
    </v-toolbar>

    <v-simple-table dense>
      <template #default>
        <thead>
          <tr>
            <th class="text-left" style="width: 40%">
              Pairing
            </th>
            <th class="text-left">
              Expectation
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Opaline x Opaline</td>
            <td>
              <ul>
                <li>100% Opaline</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Opaline Cock x Normal Hen</td>
            <td>
              <ul>
                <li>Normal/Opaline Cocks</li>
                <li>Opaline Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Opaline Cock x Opaline Hen</td>
            <td>
              <ul>
                <li>Opaline Cocks</li>
                <li>Normal/Opaline Cocks</li>
                <li>Opaline Hens</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Opaline Cock x Normal Hen</td>
            <td>
              <ul>
                <li>Normal/Opaline Cocks</li>
                <li>Normal Cocks</li>
                <li>Opaline Hens</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal Cock x Opaline Hen</td>
            <td>
              <ul>
                <li>Normal/Opaline Cocks</li>
                <li>Normal Hens</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-toolbar color="blue darken-4" class="mt-3" flat>
      <h3 class="white--text">
        Recessive Pied
      </h3>
    </v-toolbar>

    <v-simple-table dense>
      <template #default>
        <thead>
          <tr>
            <th class="text-left" style="width: 40%">
              Pairing
            </th>
            <th class="text-left">
              Expectation
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Recessive Pied x Normal</td>
            <td>
              <ul>
                <li>100% Normal/Rec Pied</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Recessive Pied x Normal/Rec Pied</td>
            <td>
              <ul>
                <li>50% Normal/Rec Pied</li>
                <li>50% Recessive Pied</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Rec Pied x Rec Pied</td>
            <td>
              <ul>
                <li>100% Rec Pied</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Rec Pied x Normal/Rec Pied</td>
            <td>
              <ul>
                <li>25% Rec Pied</li>
                <li>50% Normal/Rec Pied</li>
                <li>25% Normal</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Normal/Rec Pied x Normal</td>
            <td>
              <ul>
                <li>50% Normal/Rec Pied</li>
                <li>50% Normal</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-toolbar color="purple" class="mt-3" flat>
      <h3 class="white--text">
        Spangle
      </h3>
    </v-toolbar>

    <v-simple-table dense>
      <template #default>
        <thead>
          <tr>
            <th class="text-left" style="width: 40%">
              Pairing
            </th>
            <th class="text-left">
              Expectation
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Spangle(SF) x Normal</td>
            <td>
              <ul>
                <li>50% Spangle(SF)</li>
                <li>50% Normals</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Spangle(DF) x Normal</td>
            <td>
              <ul>
                <li>100% Spangles</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Spangle(SF) x Spangle(SF)</td>
            <td>
              <ul>
                <li>25% Spangle(DF)</li>
                <li>50% Spangle(SF)</li>
                <li>25% Normals</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Spangle(SF) x Spangle(DF)</td>
            <td>
              <ul>
                <li>50% Spangles(SF)</li>
                <li>50% Spangles(DF)</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Spangle(DF) x Spangle(DF)</td>
            <td>
              <ul>
                <li>100% Spangle(DF)</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>

    <v-toolbar color="#8F00FF" class="mt-3" flat>
      <h3 class="white--text">
        Violet
      </h3>
    </v-toolbar>

    <v-simple-table dense>
      <template #default>
        <thead>
          <tr>
            <th class="text-left" style="width: 40%">
              Pairing
            </th>
            <th class="text-left">
              Expectation
            </th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Violet(SF) Skyblue x Mauve</td>
            <td>
              <ul>
                <li>50% Violet(SF)</li>
                <li>50% Cobolt</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(DF) Skyblue x Mauve</td>
            <td>
              <ul>
                <li>100% Violet(SF) Cobolt</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(SF) Skyblue x Cobolt</td>
            <td>
              <ul>
                <li>25% Violet(SF) Cobolt</li>
                <li>25% Violet(SF) Skyblue</li>
                <li>25% Cobolt</li>
                <li>25% Skyblue</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(DF) Skyblue x Cobolt</td>
            <td>
              <ul>
                <li>50% Violet(SF) Cobolt</li>
                <li>50% Violet(SF) Skyblue</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(SF) Skyblue x Skyblue</td>
            <td>
              <ul>
                <li>50% Violet(SF) Skyblue</li>
                <li>50% Skyblue</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(DF) Cobolt x Skyblue</td>
            <td>
              <ul>
                <li>100% Violet(SF) Skyblue</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(SF) Cobolt x Skyblue</td>
            <td>
              <ul>
                <li>25% Violet(SF) Cobolt</li>
                <li>25% Violet(SF)Skyblue</li>
                <li>25% Cobolt</li>
                <li>25% Skyblue</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(DF) Cobolt x Skyblue</td>
            <td>
              <ul>
                <li>50% Violet(SF) Cobolt</li>
                <li>50% Violet (SF) Skyblue</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(SF) Cobolt x Cobolt</td>
            <td>
              <ul>
                <li>12,5% Violet(SF) Skyblue</li>
                <li>25% Violet(SF) Cobolt</li>
                <li>12,5% Violet(SF) Mauve</li>
                <li>25% Skyblue</li>
                <li>25% Mauve</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(DF) Cobolt x Cobolt</td>
            <td>
              <ul>
                <li>25% Violet(SF) Skyblue</li>
                <li>50% Violet(SF) Cobolt</li>
                <li>25% Violet(SF) Mauve</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(SF) Mauve x Skyblue</td>
            <td>
              <ul>
                <li>50% Violet(SF) Cobolt</li>
                <li>50% Cobolt</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(DF) Mauve x Skyblue</td>
            <td>
              <ul>
                <li>100% Violet(SF) Cobolt</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(SF) Mauve x Cobolt</td>
            <td>
              <ul>
                <li>25% Violet(SF) Cobolt</li>
                <li>25% Violet(SF) Mauve</li>
                <li>25% Mauve</li>
                <li>25% Cobolt</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(DF) Mauve x Cobolt</td>
            <td>
              <ul>
                <li>50% Violet(SF) Cobolt</li>
                <li>50% Violet(SF) Mauve</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(SF) Mauve x Mauve</td>
            <td>
              <ul>
                <li>50% Violet(SF) Mauve</li>
                <li>50% Mauve</li>
              </ul>
            </td>
          </tr>
          <tr>
            <td>Violet(DF) Mauve x Mauve</td>
            <td>
              <ul>
                <li>100% Violet(SF) Mauve</li>
              </ul>
            </td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>
  </v-container>
</template>

<script>
export default {
  name: 'BreedingExpectations',
  data: () => ({})
}
</script>

<style scoped>

</style>
