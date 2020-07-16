<template>
   <v-expansion-panels focusable>
    <v-expansion-panel>
      <v-expansion-panel-header>Product categories</v-expansion-panel-header>
      <v-expansion-panel-content>
        

        <v-list
          dense
          nav
        >
          <v-list-item
            link
          >
            <v-list-item-content>
              <v-list-item-title>Nike Sneakers</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

           <v-list-item 
             link
             rounded
             v-for="index in 34"
             v-bind:key="index"
           >
            <v-list-item-content>
              <v-list-item-title>Jordan {{index}}</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>


      </v-expansion-panel-content>
    </v-expansion-panel>
  </v-expansion-panels>
</template>

<script>
export default {
    data: () => ({
    })
}
</script>