<template>
  <v-app
    id="inspire"
    style="padding: 40px; background-color: transparent; width: 100%;"
  >
    <div
      class="font-weight-black white--text"
      style="font-size: xx-large; margin-bottom: 20px; padding-left: 56px;"
    >
      Credentials
    </div>

    <v-row no-gutters>
      <v-col cols="2">
        <div style="margin-right: 20%;">
          <v-text-field
            label="Access key"
            required
            style="margin-left: 20%;"
          ></v-text-field>
          <v-text-field
            label="Secret key"
            required
            style="margin-left: 20%;"
          ></v-text-field>
        </div>
      </v-col>
      <v-col cols="1"><v-divider class="mx-0" vertical dark></v-divider></v-col>
      <v-col>
        <div>
          <v-select
            label="AWS Profile"
            :items="profile"
            :rules="[(v) => !!v || 'Item is required']"
            required
            style="width: 20%;"
          ></v-select>
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
  </v-app>
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
