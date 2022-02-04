<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container class="main-container bg-background-color">
      <div class="container">
        <Header />

        <PageContent />
      </div>
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent } from "vue";
import Header from "components/Header.vue";
import PageContent from "components/PageContent.vue";

export default defineComponent({
  name: "MainLayout",

  components: { Header, PageContent },

  setup() {},
});
</script>
