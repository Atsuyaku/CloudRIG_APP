<template>
  <div style="padding-left: 56px;">
  <v-app
    id="inspire"
    style="padding: 40px; background-color: transparent; height: 400px "

  >
    <div
      class="font-weight-black white--text"
      style="font-size: xx-large; margin-bottom: 20px;"
    >
      Credentials
    </div>
    <v-row >
    <v-col cols="6">
    <v-col>
    <v-row no-gutters>
      <v-col md="4">
        <div>
          <v-text-field
            placeholder="AKIAJSIE27KKMHXI3BJQ"
            label="Access Key Id"
            required

          ></v-text-field>
        </div>
      </v-col>
      <v-col cols="1" align="center" > <div style="margin-top: 10px; width: 15px;">or</div><v-divider class="mx-0" vertical dark></v-divider></v-col>

      <v-col cols="4">
        <div>
          <v-select
            label="AWS Profile"
            :items="profile"
            :rules="[(v) => !!v || 'Item is required']"
            required

          ></v-select>
        </div>

      </v-col>

    </v-row>
    <v-row no-gutters>
      <v-col md="4">
        <div>
          <v-text-field
                  placeholder="5bEYu26084qjSFyclM/f2pz4gviSfoOg+mFwBH39"
                  label="Secret access key "
                  required

          ></v-text-field>
        </div>
      </v-col>
      </v-row>
    <v-row>

      <v-col>
        <router-link tag="span" to="/CSP">
          <v-btn dark style="margin-left: 20px;">Previous</v-btn>
        </router-link>

        <router-link tag="span" to="/MachineSumUp" style="margin-left: 31%;">
          <v-btn>NEXT</v-btn>
        </router-link>
      </v-col>

    </v-row>
    </v-col>
    </v-col>
    <v-col offset="1" cols="4" style="background-color: rgba(44, 62, 80, 0.5)" align="center">
      <v-row align="center" style="border-bottom: solid; border-color: rgba(44, 62, 80, 0.7)">
        <v-col>
          <div class="font-weight-black white--text" style="font-size: large;">
            HELP
          </div></v-col>
      </v-row>
      <v-row align="center">
        <v-col>
          <div class="font-weight-black white--text" style="font-size: large;">
          How to generate your credentials
          </div>
        </v-col>
      </v-row>
      <v-row align="center">
        <v-col>
          <div>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit,
            sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            Ut enim ad minim veniam, quis nostrud exercitation ullamco
            laboris nisi ut aliquip ex ea commodo consequat.
            Duis aute irure dolor in reprehenderit in voluptate
            velit esse cillum dolore eu fugiat nulla pariatur.
            Excepteur sint occaecat cupidatat non proident,
            sunt in culpa qui officia deserunt mollit anim id est laborum.
          </div>
        </v-col>
      </v-row>
      <v-row align="center">
        <v-col>
          <div>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit,
            sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            Ut enim ad minim veniam, quis nostrud exercitation ullamco
            laboris nisi ut aliquip ex ea commodo consequat.
            Duis aute irure dolor in reprehenderit in voluptate
            velit esse cillum dolore eu fugiat nulla pariatur.
            Excepteur sint occaecat cupidatat non proident,
            sunt in culpa qui officia deserunt mollit anim id est laborum.
          </div>
        </v-col>
      </v-row>

    </v-col>
    </v-row>
    <v-row></v-row>
    <v-row></v-row>
    <v-row></v-row>
    <v-row></v-row>
    <v-row></v-row>
    <v-row></v-row>
    <v-row></v-row>
    <v-row></v-row>
    <v-row></v-row>

  </v-app>
  </div>
</template>
<script>
export default {
  name: "CredentialsContent",
  data() {
    return {
      profile: ["profile 1", "profile 2", "profile 3", "profile 4"],
      checkbox: true,
    };
  },
};
</script>

<style scoped>

</style>
