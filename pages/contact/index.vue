<template>
  <section class="about">
    <div class="section">
      <div class="container">
        <h1 class="has-text-dark page-title">
          Contact
        </h1>
        <ContactForm />
      </div>
    </div>
    <div class="bottom-hero">
      <img src="~/assets/img/contact-hero-bg.jpg" alt />
    </div>
  </section>
</template>
<script>
import ContactForm from "~/components/ContactForm";
export default {
  name: "Contact",
  components: {
    ContactForm
  }
};
</script>
