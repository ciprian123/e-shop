<template>
  <v-container fluid>
    <v-row 
      align="center"
      justify="start"
    >
    <v-col cols="3" md="3" sm="6" xs="6">
      <Product name="Bormasina" price="123 RON" image="https://picsum.photos/240/140"/>
    </v-col>
    <v-col cols="3" md="3" sm="6" xs="6">
      <Product name="Smart TV" price="234 RON" image="https://picsum.photos/240/140"/>
    </v-col>
    <v-col cols="3" md="3" sm="6" xs="6">
      <Product name="Smart Fridge" price="1000 RON" image="https://picsum.photos/240/140"/>
    </v-col>
    <v-col cols="3" md="3" sm="6" xs="6">
      <Product name="Smart Fridge" price="1000 RON" image="https://picsum.photos/240/140"/>
    </v-col>
    <v-col cols="3" md="3" sm="6" xs="6">
      <Product name="Smart Fridge" price="1000 RON" image="https://picsum.photos/240/140"/>
    </v-col>
    <v-col cols="3" md="3" sm="6" xs="6">
      <Product name="Smart Fridge" price="1000 RON" image="https://picsum.photos/240/140"/>
    </v-col>
    <v-col cols="3" md="3" sm="6" xs="6">
      <Product name="Smart Fridge" price="1000 RON" image="https://picsum.photos/240/140"/>
    </v-col>
    <v-col cols="3" md="3" sm="6" xs="6">
      <Product name="Smart Fridge" price="1000 RON" image="https://picsum.photos/240/140"/>
    </v-col>
    <v-col cols="3" md="3" sm="6" xs="6">
      <Product name="Smart Fridge" price="1000 RON" image="https://picsum.photos/240/140"/>
    </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Product from "../components/Product.vue"

export default {
  components: {
    Product
  }
};
</script>
