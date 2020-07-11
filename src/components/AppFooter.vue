<template>
  <v-footer
    color="primary lighten-1"
    padless
    class="mt-15"
  >
    <v-row
      justify="center"
      no-gutters
    >
      <v-btn
        v-for="link in links"
        :key="link"
        color="white"
        text
        rounded
        class="my-2"
      >
        {{ link }}
      </v-btn>
      <v-col
        class="primary lighten-2 py-4 text-center white--text"
        cols="12"
      >
        <strong>{{ new Date().getFullYear() }} — Made &amp; design by Ciprian Ursulean</strong>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      links: [
        'Terms and conditions',
        'Orders and shipment',
        'About us',
        'Client support',
        'Contact Us',
      ],
    }),
  }
</script>