<template>
  <v-container class="MachineCreationContent">
    <v-layout
      column
      pa-10
      style="padding-top: 40px; padding-left: 40px; width: 50%;"
    >
      <div style="padding-left: 56px;">
        <div
          class="font-weight-black white--text"
          style="font-size: xx-large; margin-bottom: 20px;"
        >
          Create a machine
        </div>
        <div>
          <v-row>
            <v-col>
              <v-text-field
                dark
                label="Name"
                v-model="name"
                :rules="nameRules"
                :counter="20"
                required
                style="width: 200px;"
              ></v-text-field>
            </v-col>
            <v-col>
              <v-select
                dark
                label="Region"
                v-model="select"
                :items="regions"
                :rules="[(v) => !!v || 'Item is required']"
                required
                style="width: 200px;"
              ></v-select>
            </v-col>
          </v-row>
          <v-textarea
            dark
            style="width: 460px;"
            label="Description"
          ></v-textarea>
          <router-link tag="button" to="/CSP">
            <v-btn
              dark
              style="margin-right: 20px;"
              @click="submit"
              :class="{ red: !valid, green: !valid }"
              >submit</v-btn
            >
          </router-link>
          <router-link tag="button" to="/">
            <v-btn dark>Cancel</v-btn>
          </router-link>
        </div>
      </div>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "MachineCreationContent",
  data() {
    return {
      valid: false,
      name: "Machine001",
      nameRules: [
        (v) => !!v || "Name is required",
        (v) => (v && v.length <= 20) || "Name must be less than 10 characters",
      ],
      select: null,
      regions: ["Europe East", "Europe West", "North America", "South America"],
    };
  },
  methods: {
    submit() {
      this.$refs.form.validate();
    },
    clear() {
      this.$refs.form.reset();
    },
  },
};
</script>

<style scoped></style>
