<template>
  <v-container fill-height class="home-content">
    <v-layout column pa-10 style="padding-left: 20px;">
      <v-row no-gutters>
        <v-col offset="5">
          <div
            class="font-weight-black white--text"
            style="
              font-size: xx-large;
              padding-bottom: 40px;
              padding-top: 30px;
            "
          >
            My Computers
          </div>
        </v-col>
      </v-row>

      <v-row>
        <v-col cols="2">
          <router-link tag="span" to="/MachineCreation">
            <v-btn
              dark
              depressed
              style="
                background-color: transparent;
                border: dashed;
                opacity: 0.6;
              "
              height="150px"
              width="150px"
              class="white"
            >
              <v-icon color="white" size="80">fas fa-plus</v-icon>
            </v-btn>
          </router-link>
        </v-col>
      </v-row>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "HomeContent",
};
</script>

<style scoped>
</style>
