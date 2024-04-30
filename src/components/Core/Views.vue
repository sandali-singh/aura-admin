<template>
  <v-main class="ma-0" style="background-color: #F5F8FC;">
    <v-container
      fluid
      class="white"
      style="height: 100% !important; border-radius: 20px !important"
    >
      <v-row align="center" justify="center">
        <v-col md="11" class="mt-10">
          <v-slide-y-reverse-transition>
            <router-view v-show="show" />
          </v-slide-y-reverse-transition>
        </v-col>
      </v-row>
    </v-container>
  </v-main>
</template>

<script>
export default {
  name: "MainView",
  data: () => ({
    show: false,
  }),
  created() {
    this.show = true;
  },
};
</script>