<template>
  <v-divider class=mt-2></v-divider>
      <v-toolbar color="transparent">
        <v-toolbar-title>LOUNGE CHAIRS</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn variant="text" color="grey">Sort by :</v-btn>
        <v-btn variant="text" color="">Name</v-btn>
        <v-btn variant="text" color="grey">Popularity</v-btn>
        <v-btn variant="text" color="grey">Price</v-btn>
      </v-toolbar>
      <v-row>
          <v-col cols="12" sm="3" v-for="(chair,i) in chairs" :key="i" >
              <v-card height="300" align="center" flat outlined tile>
                <v-img :src="chair.image" width="200" height="200" contain></v-img>
                <v-card-text class="mt-n1">
                  <strong>{{chair.title}}</strong>
                </v-card-text>
                <v-card-text class="mt-n4">
                  <strong>{{chair.price}}</strong>
                </v-card-text>
              </v-card>
          </v-col>
      </v-row>
      <v-divider></v-divider>
      <v-toolbar color="transparent">
        <v-toolbar-title class="text-caption">Show more chairs</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-icon color="grey" left class="mr-4 mt-n1">fas fa-long-arrow-alt-left</v-icon>
        <span class="text-caption">3</span>
        <v-icon color="grey" left class="ml-4 mt-n1 mr-2">fas fa-long-arrow-alt-right</v-icon>
      </v-toolbar>
</template>

<script>
export default {
    setup(){
  return {

    chairs:[
    {
          class: "pa-0",
          image: "c1.jpg",
          title: "Lounge Chair",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c2.jpg",
          title: "Repos",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c3.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c4.png",
          title: "Loby Chair",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c5.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c6.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c7.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c8.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c9.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c10.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c11.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c12.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c13.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c14.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c15.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
        {
          class: "pa-0",
          image: "c16.png",
          title: "Modern Lounge",
          price: "$ 145.00",
        },
    ]
  }
}, 
}
</script>

<style>

</style>