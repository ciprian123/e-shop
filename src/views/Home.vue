<template>
  <v-col cols="12">
    <Product name="Bormasina" price="123 RON" image="https://picsum.photos/240/140"/>
    <Product name="Smart TV" price="234 RON" image="https://picsum.photos/240/140"/>
  </v-col>
</template>

<script>
import Product from "../components/Product.vue"

export default {
  components: {
    Product
  }
};
</script>
