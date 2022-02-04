<template>
  <div class="main-content">
    <div class="first-column">
      <div class="title">
        <h2><span>Bee</span>p Us</h2>
        <a href="#">info@uxtweak.com</a>
        <div class="title-small-text">
          <h3>Office</h3>
          <p>
            UXtweak j.s.a., Obchodna 58, 811 06 Bratislava Slovakia (European
            Union)
          </p>
        </div>
      </div>
      <div class="schedule-link card">
        <h2>Schedule a Live Demo</h2>
        <button class="schedule-btn">Schedule</button>
      </div>
    </div>
    <div class="second-column">
      <div class="form-title">
        <h1>Contact Us</h1>
        <h3>Feel free to send us a message</h3>
      </div>

      <div class="form-container card">
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
            :rules="[
              (val) => (val && val.length > 0) || 'Please type something',
            ]"
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
            :rules="[
              (val) => (val && val.length > 0) || 'Please type something',
            ]"
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

        <div class="form-text">
          <p>
            This site is protected by reCAPTCHA and the Google
            <a href="#">Privacy Policy</a> and
            <a href="#">Terms of Service</a> apply
          </p>
        </div>

        <div class="btn-container">
          <q-btn
            padding="10px 0"
            no-caps
            style="background: #f0c002; width: 100%"
            text-color="white"
          >
            <div class="btn-send">Send</div>
          </q-btn>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "PageContent",

  components: {},

  setup() {},
});
</script>
