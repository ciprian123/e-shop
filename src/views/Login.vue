<template>
  <v-main>
    <v-container class="fill-height mt-12" fluid>
      <v-row align="center" justify="center">
        <v-col cols="12" sm="8" md="4">
          <v-card class="elevation-12">
            <v-toolbar color="accent" dark flat>
              <v-toolbar-title>Welcome back</v-toolbar-title>
              <v-spacer></v-spacer>
              </v-toolbar>
                <v-card-text>
                  <v-form>
                    <v-text-field
                      label="Login"
                      name="login"
                      prepend-icon="mdi-account"
                      type="text"
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
                  </v-form>
                </v-card-text>
                <v-card-actions>
                  <v-btn color="primary">Login</v-btn>
                  <v-spacer></v-spacer>
                  <v-btn color="primary">Forgot password?</v-btn>
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