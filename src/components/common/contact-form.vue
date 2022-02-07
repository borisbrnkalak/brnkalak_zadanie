<template>
  <q-form @submit="onSubmit" @reset="onReset" class="q-gutter-md">
    <q-input
      outlined
      color="yellow-9"
      label-color="gray"
      v-model="name"
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
      v-model="email"
      label="Your email *"
      hint="Email"
      lazy-rules
      :rules="[(val) => (val && val.length > 0) || 'Please type something']"
    />

    <q-input
      v-model="text"
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
