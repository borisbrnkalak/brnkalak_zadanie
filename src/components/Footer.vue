<template>
  <footer class="main-footer">
    <div class="links-wrapper">
      <ul class="column-lists" v-for="link in links" v-bind:key="link.name">
        <li class="list-title">{{ link.name }}</li>
        <ul class="specific-lists">
          <li
            class="specific-links"
            v-for="item in link.items"
            v-bind:key="item"
          >
            <q-btn
              no-caps
              flat
              align="left"
              bg-color="transparent"
              class="full-width"
            >
              {{ item }}
            </q-btn>
          </li>
        </ul>
      </ul>
    </div>
    <div class="copyright">
      <p>Copyright © 2021 UXtweak Research Group. All rights reserved.</p>
    </div>
  </footer>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "Footer",

  components: {},

  setup() {
    const links = [
      {
        name: "Product",
        items: ["Features", "Pricing", "Demos", "Consulting"],
      },
      {
        name: "Resources",
        items: ["Documentation", "Performance"],
      },
      {
        name: "Legal",
        items: [
          "Privacy policy",
          "GDPR compliance",
          "Terms of service",
          "Privacy policy",
          "Opt-out",
          "DPA",
        ],
      },
      {
        name: "Company",
        items: ["Contact form", "Blog", "Careers"],
      },
    ];
    return { links };
  },
});
</script>
