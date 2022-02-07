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
        <q-btn no-caps color="white" text-color="grey-7" label="Schedule" />
      </div>
    </div>
    <div class="second-column">
      <HeadingTitle
        mainTitle="Contact us"
        subTitle="Feel free to send us a message"
      />
      <div class="form-container card">
        <ContactForm />

        <div class="form-text">
          <p>
            This site is protected by reCAPTCHA and the Google
            <a href="#">Privacy Policy</a> and
            <a href="#">Terms of Service</a> apply
          </p>
        </div>

        <div class="btn-container">
          <SendButton btnContent="Send" btnColor="amber-7" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import SendButton from "components/common/c-btn.vue";
import ContactForm from "components/common/contact-form.vue";
import HeadingTitle from "components/common/heading-title.vue";

export default defineComponent({
  name: "PageContent",

  components: { SendButton, ContactForm, HeadingTitle },

  setup() {},
});
</script>
