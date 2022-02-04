<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container class="main-container bg-background-color">
      <div class="container">
        <Header />

        <PageContent />

        <Footer />
      </div>
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent } from "vue";
import Header from "components/Header.vue";
import PageContent from "components/PageContent.vue";
import Footer from "components/Footer.vue";

export default defineComponent({
  name: "MainLayout",

  components: { Header, PageContent, Footer },

  setup() {},
});
</script>
