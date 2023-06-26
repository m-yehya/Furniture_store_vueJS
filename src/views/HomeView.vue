<template>
  <v-app>
    <NavBar />
    <v-container fluid>
      <ProductCategoriesVue/>
      <ProductsFilter/>
      <ProductsDisplay/>
    </v-container>
    <FooterView />
  </v-app>
</template>

<script>
import { defineComponent } from 'vue';

// Components
import NavBar from '@/components/NavBar.vue';
import FooterView from '@/components/FooterView.vue';
import ProductsFilter from '@/components/ProductsFilter.vue';
import ProductCategoriesVue from '@/components/ProductCategories.vue';
import ProductsDisplay from '@/components/ProductsDisplay.vue';
export default defineComponent({
  name: 'HomeView',
  components: {
    NavBar,
    ProductCategoriesVue,
    ProductsFilter,
    ProductsDisplay,
    FooterView
},
});
</script>
<style scoped>
  .v-container{
    width: 100%;
    padding: 16px 0px !important;
    margin-right: auto;
    margin-left: auto;
  }
  .v-card.borderme {
    border: 2px solid black !important;
  }
  .v-card.borderout {
    border: 1px solid #d5f0db !important;
  }
</style>