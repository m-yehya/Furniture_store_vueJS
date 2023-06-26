<template>
  <v-card

        color="#F7F7F7"
        tile
        flat
        class="d-flex align-center justify-center mt-12"
        dark
      >
        <v-row >
          <v-col cols="12" sm="12" >
            <v-item-group mandatory class="mt-n1">
              <v-container>
                <v-row justify="center" class="space">
                  <v-col
                    cols="5"
                    xs="12"
                    sm="4"
                    md="2"
                    v-for="(cetegory, i) in categories"
                    :key="i"
                  >
                    <v-item v-slot="{ active, toggle }">
                      <v-card
                        :color="active ? '#D5F0DB' : 'white'"
                        :class="active ? 'borderme' : 'borderout'"
                        class="d-flex align-center rounded-lg mx-2"
                        dark
                        height="170"
                        @click="toggle"
                        flat
                      >
                        <v-row>
                          <v-col cols="12" sm="12" >
                            <v-list-item three-line class="text-center" >
                              <v-list-item-content>
                                <div align="center" justify="center">
                                  <v-img
                                    :src="cetegory.img"
                                    max-height="80"
                                    max-width="80"
                                    contain
                                  ></v-img>
                                </div>
                                <v-list-item-subtitle
                                  :class="
                                    active ? 'green--text' : 'black--text'
                                  "
                                  class="caption mt-4"
                                  >{{ cetegory.title }}</v-list-item-subtitle
                                >
                              </v-list-item-content>
                            </v-list-item>
                          </v-col>
                        </v-row>
                      </v-card>
                    </v-item>
                  </v-col>
                </v-row>
              </v-container>
            </v-item-group>
          </v-col>
        </v-row>
      </v-card>
</template>

<script>
export default {
setup(){
    return{
        categories: [
    { img: "9.png", title: "SLEEPING BEDS" },
        { img: "2.png", title: "LOUNGE CHAIRS" },
        { img: "1.png", title: "CHAIRS" },
        { img: "4.png", title: "OFFICE CHAIRS" },
        { img: "8.jpg", title: "TABLES NIGHTSTANDS" },
        { img: "6.png", title: "KITCHEN FURNITURE" },
    ]
    }  
}
}
</script>

<style>

</style>