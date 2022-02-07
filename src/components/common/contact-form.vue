<template>
  <q-form class="q-gutter-md">
    <q-input
      outlined
      color="yellow-9"
      label-color="gray"
      label="Your name *"
      hint="Name and surname"
      lazy-rules
      bg-color="white"
      :rules="[(val) => (val && val.length > 0) || 'Please type something']"
    />

    <q-input
      outlined
      type="email"
      color="yellow-9"
      label-color="gray"
      bg-color="white"
      label="Your email *"
      hint="Email"
      lazy-rules
      :rules="[(val) => (val && val.length > 0) || 'Please type something']"
    />

    <q-input
      outlined
      color="yellow-9"
      label-color="gray"
      bg-color="white"
      type="textarea"
      label="Your message *"
      hint="Message"
    />
  </q-form>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "ContactForm",

  props: [""],

  setup() {},
});
</script>
