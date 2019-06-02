<template>
  <footer class="footer">
    <div class="content has-text-centered">
      <div v-if="this.$route.path === '/'" class="contact-form--footer">
        <p class="has-text-weight-bold">Don’t see what you’re looking for?</p>
        <p class="has-text-weight-bold">
          Contact me with details. If I can’t assist, I’ll refer you to someone
          who can.
        </p>
        <ContactForm />
      </div>

      <p>&copy; {{ date }} Kaitlyn Jasmin</p>
    </div>
  </footer>
</template>

<script>
import ContactForm from "~/components/ContactForm";
export default {
  name: "Footer",
  components: {
    ContactForm
  },
  data() {
    return {
      date: new Date().getFullYear()
    };
  }
};
</script>
