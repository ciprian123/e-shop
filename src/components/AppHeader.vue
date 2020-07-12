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

      <v-menu offset-y>
      <template v-slot:activator="{ on, attrs }">
        <v-btn icon
          dark
          v-bind="attrs"
          v-on="on"
        >
          <v-icon>account_circle</v-icon>
        </v-btn>
      </template>
      <v-list>
        <v-list-item link to='/login'>
          <v-list-item-title>Sign in</v-list-item-title>
        </v-list-item>
        <v-list-item link to='signup'>
          <v-list-item-title>Sign up</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>

      <v-btn icon>
        <v-icon>favorite</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>local_mall</v-icon>
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
              <v-icon>mdi-help</v-icon>
            </v-list-item-action>
            <v-list-item-content>
              <v-list-item-title>About us</v-list-item-title>
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
        <AppSidenav/>
      </v-navigation-drawer>
  </section>
</template>

<script> 
  import AppSidenav from "./AppSidenav.vue"

  export default {
    data: () => ({
      drawer: null,
      headerOptions: ['account_circle', 'favorite', 'local_mall']
    }),
    components: {
      AppSidenav
    }
  }
</script>