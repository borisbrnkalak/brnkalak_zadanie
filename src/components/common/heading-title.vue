<template>
  <div class="form-title">
    <h1>{{ mainTitle }}</h1>
    <h3>{{ subTitle }}</h3>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HeadingTitle",

  props: ["mainTitle", "subTitle"],

  setup() {},
});
</script>
