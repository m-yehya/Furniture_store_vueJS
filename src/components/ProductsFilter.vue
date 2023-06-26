<template>
    <v-row class="column-pairs">
      <v-col cols="12" md="2"  class="column-with-line">
        <v-checkbox v-model="chair" label="Chairs" class="check mt-4 centered-element " ></v-checkbox>
      </v-col>
      <v-col cols="12" md="2" class="column-with-line">
        <v-checkbox v-model="other" label="Other" class="check mt-4 centered-element"></v-checkbox>
      </v-col>
      <v-col cols="12" md="2" class="column-with-line">
        <div class="centered-container">
        <v-btn variant="text" class="centered-element">Leather Colors
            <v-icon right class="ml-2 mt-n1">fas fa-caret-right</v-icon>
          </v-btn>
        </div>
      </v-col>
      <v-col cols="12" md="2" class="column-with-line">
        <div class="centered-container">
        <v-btn variant="text">Choose Design
            <v-icon right class="ml-2 mt-n1">fas fa-caret-right</v-icon>
          </v-btn>
          </div>
      </v-col>
      <v-col cols="12" md="4"  class="column-with-line">
        <div class="flex-container centered-container" >
          <span class="text-caption mx-6">Price till</span>
          <v-slider v-model="slider2"  class="mt-5 "></v-slider>
          <span class="text-caption mx-6 ">$9,700</span>
        </div>
      </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      chair: true,
      slider2: 50,
    };
  },
}
</script>

<style>
.column-with-line {
  border-right: 1px solid #ccc;
  padding-right: 10px;
}
.centered-element {
  display: flex;
  align-items: center;
  justify-content: center;
}
.flex-container {
  display: flex;
  align-items: center;
}
.centered-container {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
}

</style>

