<template>
  <div id="app" style="padding-left: 56px;">
    <v-app
      id="inspire"
      style="padding: 40px; background-color: transparent; width: 100%;"
    >
      <div
        class="font-weight-black white--text"
        style="font-size: xx-large; margin-bottom: 20px;"
        align="center"
      >
        Credentials
      </div>
      <v-row no-gutters justify="center">
        <v-col>
          <div style="margin-left: 30px;" align="center">
            <v-text-field
              label="Access key"
              required
              style="width: 25%;"
            ></v-text-field>

            <v-text-field
              label="Secret key"
              required
              style="width: 25%;"
            ></v-text-field>

            <v-col style="margin-left: 90%; margin-top: 30%;">
              <router-link tag="span" to="/">
                <v-btn>NEXT</v-btn>
              </router-link>
            </v-col>
          </div>
        </v-col>
        <v-col>
          <div align="center">
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
