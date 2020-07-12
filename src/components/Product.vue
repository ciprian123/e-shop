<template>
  <v-card
    class="mx-auto mt-5"
    max-width="240"
  >
    <v-img
      :src="image"
      height="140px"
    ></v-img>


    <v-card-title class="accent--text">
      {{ name }}
    </v-card-title>

    <v-card-actions>
      <v-btn text icon><v-icon>local_mall</v-icon></v-btn>
      <v-spacer></v-spacer>
      <v-card-title class="primary--text justify-center">
      {{ price }}
      </v-card-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>favorite</v-icon>
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  data: () => ({

  }),
  props: {
    name: {
      type: String,
      required: true
    },
    price: {
      type: String,
      required: true
    },
    image: {
      type: String,
      required: true
    }
  }
}
</script>