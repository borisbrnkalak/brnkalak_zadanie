<template>
  <li class="specific-link">
    <div class="arrow-text">
      <a href="#">{{ linkContent }}</a>
      <i v-if="isDropdown" class="fas fa-caret-down"></i>
    </div>
    <div v-if="isDropdown" class="sub-post">
      <slot></slot>
    </div>
  </li>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HeaderLinkElement",

  props: {
    isDropdown: Boolean,
    linkContent: String,
  },

  setup() {},
});
</script>
