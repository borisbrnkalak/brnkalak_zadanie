<template>
  <header class="main-header">
    <div class="navigation-links">
      <div class="openMenu">
        <div :class="'menu-btn ' + (isMobile ? 'open' : '')" @click="btnMenu">
          <div class="menu-btn__burger"></div>
        </div>
      </div>
      <HeaderLinks :isMobile="isMobile" :btnMenu="btnMenu" />
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
import { defineComponent, ref } from "vue";
import HeaderLinks from "components/common/header-links.vue";

export default defineComponent({
  name: "Header",

  components: { HeaderLinks },

  setup() {
    const isMobile = ref(false);
    const reveal = function () {};
    const btnMenu = () => {
      isMobile.value = !isMobile.value;
    };
    return { isMobile, btnMenu };
  },
});
</script>
