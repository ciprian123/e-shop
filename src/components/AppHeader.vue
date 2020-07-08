<template>
  <section>
    <v-app-bar
      color="primary"
      dark
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>Ciprian's store</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-text-field
          center
          solo-inverted
          flat
          hide-details
          label="Search"
          prepend-inner-icon="search"
        ></v-text-field>
      <v-spacer></v-spacer>
      <v-btn icon
        v-for='option in headerOptions'
        v-bind:key='option'>
        <v-icon>{{ option }}</v-icon>
      </v-btn>
    </v-app-bar>
    

     <v-navigation-drawer
        v-model="drawer"
        app
        temporary
      >
        <v-list dense>
          <v-list-item link>
            <v-list-item-action>
              <v-icon>mdi-home</v-icon>
            </v-list-item-action>
            <v-list-item-content>
              <v-list-item-title>Home</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item link>
            <v-list-item-action>
              <v-icon>mdi-email</v-icon>
            </v-list-item-action>
            <v-list-item-content>
              <v-list-item-title>Contact</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
  </section>
</template>

<script>
  export default {
    data: () => ({
      drawer: null,
      headerOptions: ['account_circle', 'favorite', 'local_mall']
    }),
    props: {
      source: String
    }
  }
</script>