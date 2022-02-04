<template>
  <header class="main-header">
    <div class="navigation-links">
      <ul class="links">
        <li class="specific-link features">
          <div class="arrow-text">
            <a href="#">Features</a>
            <i class="fas fa-caret-down"></i>
          </div>
          <div class="sub-post">
            <div class="sub-post-content">
              <div class="first-column">
                <h3>Contact Form</h3>
                <p>Feel free to send us a message</p>
              </div>
              <div class="second-column">
                <h3>Schedule a Live Demo</h3>
                <p>Books a live demo with our product specialist</p>
              </div>
            </div>
          </div>
        </li>
        <li class="specific-link pricing"><a href="#">Pricing</a></li>
        <li class="specific-link contact">
          <div class="arrow-text">
            <a href="#">Contact</a>
            <i class="fas fa-caret-down"></i>
          </div>
          <div class="sub-post">
            <div class="sub-post-content">
              <div class="first-column">
                <h3>Contact Form</h3>
                <p>Feel free to send us a message</p>
              </div>
              <div class="second-column">
                <h3>Schedule a Live Demo</h3>
                <p>Books a live demo with our product specialist</p>
              </div>
            </div>
          </div>
        </li>
        <li class="specific-link learn">
          <div class="arrow-text">
            <a href="#">Learn</a>
            <i class="fas fa-caret-down"></i>
          </div>
        </li>
      </ul>
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

export default defineComponent({
  name: "Header",

  components: {},

  setup() {},
});
</script>
