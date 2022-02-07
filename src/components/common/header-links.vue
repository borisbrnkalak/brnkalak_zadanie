<template>
  <ul class="links">
    <HeaderLinkElement isDropdown linkContent="Features"
      ><div class="sub-post-content">
        <!--Alebo tu mozu ist ine komponenty, vlastne -->
        <div class="first-column">
          <h3>Contact Form</h3>
          <p>Feel free to send us a message</p>
        </div>
        <div class="second-column">
          <h3>Schedule a Live Demo</h3>
          <p>Books a live demo with our product specialist</p>
        </div>
      </div></HeaderLinkElement
    >
    <HeaderLinkElement linkContent="Pricing" />
    <HeaderLinkElement isDropdown linkContent="Contact"
      ><div class="sub-post-content">
        <!--Alebo tu mozu ist ine komponenty, vlastne -->
        <div class="first-column">
          <h3>Contact Form</h3>
          <p>Feel free to send us a message</p>
        </div>
        <div class="second-column">
          <h3>Schedule a Live Demo</h3>
          <p>Books a live demo with our product specialist</p>
        </div>
      </div></HeaderLinkElement
    >
    <HeaderLinkElement isDropdown linkContent="Learn"
      ><div class="sub-post-content">
        <!--Alebo tu mozu ist ine komponenty, vlastne -->
        <div class="first-column">
          <h3>Contact Form</h3>
          <p>Feel free to send us a message</p>
        </div>
        <div class="second-column">
          <h3>Schedule a Live Demo</h3>
          <p>Books a live demo with our product specialist</p>
        </div>
      </div></HeaderLinkElement
    >
  </ul>
</template>

<script>
import { defineComponent } from "vue";
import HeaderLinkElement from "components/common/header-link-elements.vue";

export default defineComponent({
  name: "HeaderLinks",

  components: { HeaderLinkElement },
  props: [""],

  setup() {},
});
</script>
