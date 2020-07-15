<template>
  <div style="padding-left: 56px;">
  <v-app
    id="inspire"
    style="padding: 40px; background-color: transparent;"
  >
    <div
      class="font-weight-black white--text"
      style="font-size: xx-large; margin-bottom: 20px;"
    >
      Credentials
    </div>
    <v-col>
    <v-row no-gutters>
      <v-col md="2">
        <div>
          <v-text-field
            label="Access key"
            required

          ></v-text-field>
        </div>
      </v-col>
      <v-col cols="1" align="center" > <div style="margin-top: 10px; width: 15px;">or</div><v-divider class="mx-0" vertical dark></v-divider></v-col>

      <v-col cols="2">
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
      <v-col cols="2" xs="3">
        <div>
          <v-text-field
                  label="Secret key"
                  required

          ></v-text-field>
        </div>
      </v-col>
      </v-row>
    <v-row>
      <v-col style="margin-left: 35%;">
        <router-link tag="span" to="/">
          <v-btn>NEXT</v-btn>
        </router-link>
      </v-col>
    </v-row>
    <v-row></v-row>
    <v-row></v-row>
    <v-row></v-row>
    <v-row></v-row>
    <v-row></v-row>
    </v-col>
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

<style scoped></style>
