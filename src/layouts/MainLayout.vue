<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container class="main-container bg-background-color">
      <div class="container">
        <Header />

        <p class="bg-yellow">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil, alias!
          Tempora aspernatur dicta molestias porro dolorum veniam officiis
          praesentium aut temporibus? Laudantium, laboriosam placeat dolorum at
          est ipsum optio nihil!
        </p>
      </div>
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent } from "vue";
import Header from "components/Header.vue";

export default defineComponent({
  name: "MainLayout",

  components: { Header },

  setup() {},
});
</script>
