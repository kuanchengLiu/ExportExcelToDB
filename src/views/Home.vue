<template>
  <v-app>
    <keep-alive>
      <DatabaseChoser></DatabaseChoser>
    </keep-alive>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";
import DatabaseChoser from "../components/DatabaseChooser.vue";

export default Vue.extend({
  name: "Home",

  components: {
    DatabaseChoser,
  },
});
</script>
