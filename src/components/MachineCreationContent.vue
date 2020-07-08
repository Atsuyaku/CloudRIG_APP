<template>
  <div style="padding-left: 56px;">
    <v-app

      style="padding: 40px; background-color: transparent; width: 50%;"
    >
      <div
        class="font-weight-black white--text"
        style="font-size: xx-large; margin-bottom: 20px;"
      >
        Create a machine
      </div>
      <div style="margin-left: 30px;">
        <v-text-field
          label="Name"
          v-model="name"
          :rules="nameRules"
          :counter="20"
          required
          style="width: 25%;"
        ></v-text-field>
        <v-textarea style="width: 50%;" label="Description"></v-textarea>
        <v-select
          label="Region"
          v-model="select"
          :items="regions"
          :rules="[(v) => !!v || 'Item is required']"
          required
          style="width: 20%;"
        ></v-select>
        <router-link tag="button" to="/CSP">
          <v-btn
            style="margin-right: 20px;"
            @click="submit"
            :class="{ red: !valid, green: !valid }"
            >submit</v-btn
          >
        </router-link>
        <v-btn @click="clear">clear</v-btn>
      </div>
    </v-app>
  </div>
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
