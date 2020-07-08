<template>
  <v-container fill-height class="CSPContent">
    <v-layout column pa-10>
      <v-row no-gutters>
        <v-col>
          <div
            class="font-weight-black white--text"
            style="font-size: xx-large; margin-bottom: 70px;"
          >
            Select your cloud provider
          </div>
        </v-col>
      </v-row>

      <v-row>
        <v-col cols="2">
          <router-link tag="span" to="/Credentials">
            <v-btn
              dark
              depressed
              class="white"
              style="background-color: transparent; border: dashed; opacity: 0.6;"
              height="170px"
              width="170px"
            >
              <v-icon color="white" size="100">
                fab fa-aws
              </v-icon>
            </v-btn>
          </router-link>
          <router-link  tag="span" to="/MachineCreation">
            <v-btn dark style="margin-top: 100px;">Previous</v-btn>
          </router-link>
        </v-col>

        <v-col cols="2">
          <router-link tag="span" to="/Credentials" >
            <v-btn
              dark
              depressed
              style="background-color: transparent; border: dashed; opacity: 0.6;"
              height="170px"
              width="170px"
              class="white"
              disabled
            >
              <v-img
                      :src="require('../assets/icons-azur.svg')"
                      contain
                      height="130"

              />
            </v-btn>
          </router-link>
        </v-col>
        <v-col cols="2">
          <router-link tag="span" to="/Credentials">
            <v-btn  v-bind="attrs" v-on="on"
              dark
              depressed
              style="background-color: transparent; border: dashed; opacity: 0.6;"
              height="170px"
              width="170px"
              class="white"
              disabled

            >
              <v-img
                      :src="require('../assets/icons-google-cloud-platform.svg')"
                      contain
                      height="130"
              />
            </v-btn>
          </router-link>
        </v-col>

        <v-col cols="2">
          <router-link tag="span" to="/Credentials">
            <v-btn
              dark
              depressed
              style="background-color: transparent; border: dashed; opacity: 0.6;"
              height="170px"
              width="170px"
              class="white"
              disabled

            >
              <p>Not available yet</p>
              <v-icon color="white" size="150"></v-icon>
            </v-btn>
          </router-link>
        </v-col>
      </v-row>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "CSPContent",
};
</script>

<style scoped></style>
