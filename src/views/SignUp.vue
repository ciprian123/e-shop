<template>
  <v-main>
    <v-container class="fill-height mt-12" fluid>
      <v-row align="center" justify="center">
        <v-col cols="12" sm="8" md="4">
          <v-card class="elevation-12">
            <v-toolbar color="accent" dark flat>
              <v-toolbar-title>Please sign up</v-toolbar-title>
              </v-toolbar>
                <v-card-text>
                  <v-form>
                    <v-text-field
                      label="First name"
                      name="fname"
                      type="text"
                      prepend-icon="person"
                    ></v-text-field>

                    <v-text-field
                      label="Last name"
                      name="lname"
                      type="text"
                      prepend-icon="person"
                    ></v-text-field>

                    <v-text-field
                      label="Email"
                      name="email"
                      type="email"
                      prepend-icon="local_post_office"
                    ></v-text-field>

                    <v-text-field
                      id="password"
                      label="Password"
                      name="password"
                      prepend-icon="mdi-lock"
                      :append-icon="showPassFlag ? 'visibility' : 'visibility_off'"
                      @click:append="() => (showPassFlag = !showPassFlag)"
                      :type="showPassFlag ? 'password' : 'text'"
                    ></v-text-field>

                    <v-text-field
                      id="password"
                      label="Confirm password"
                      name="password"
                      prepend-icon="mdi-lock"
                      :append-icon="showPassFlag ? 'visibility' : 'visibility_off'"
                      @click:append="() => (showPassFlag = !showPassFlag)"
                      :type="showPassFlag ? 'password' : 'text'"
                    ></v-text-field>

                    <v-text-field
                      label="Phone number"
                      name="phone-nr"
                      type="text"
                      prepend-icon="local_phone"
                    ></v-text-field>

                    <v-text-field
                      label="Address"
                      name="address"
                      type="text"
                      prepend-icon="public"
                    ></v-text-field>
                  </v-form>
                </v-card-text>
                <v-card-actions class="justify-center">
                  <v-btn class="mb-5" color="primary">Sign up</v-btn>
                </v-card-actions>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </v-main>
</template>

<script>
export default {
    data: () => ({
        showPassFlag: true
    })
}
</script>