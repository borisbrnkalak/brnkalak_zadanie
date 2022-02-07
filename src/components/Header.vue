<template>
  <header class="main-header">
    <div class="navigation-links">
      <div class="nav-icon" v-if="mobileView"></div>
      <HeaderLinks v-if="!mobileView" />
    </div>

    <div class="login-btns">
      <div class="register">
        <button class="register-btn">
          <div class="content">
            <span class="large">Register</span>
            <span class="tiny">for free</span>
          </div>
        </button>
      </div>

      <div class="login">
        <button class="login-btn"><span class="large">Log In</span></button>
      </div>
    </div>
  </header>
</template>

<script>
import { defineComponent } from "vue";
import HeaderLinks from "components/common/header-links.vue";

export default defineComponent({
  name: "Header",

  components: { HeaderLinks },

  setup() {
    if (window.innerWidth <= 955) {
      console.log("aaa");
    }
  },
});
</script>
