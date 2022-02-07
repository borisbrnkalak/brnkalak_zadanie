<template>
  <q-btn
    padding="10px 0"
    no-caps
    style="width: 100%"
    :color="btnColor"
    text-color="white"
  >
    <div class="btn-send">{{ btnContent }}</div>
  </q-btn>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "SendButton",

  props: ["btnContent", "btnColor"],

  setup() {},
});
</script>
