<template>
  <nav
    class="navbar is-fixed-top"
    :class="{ 'is-active': mobile_menu }"
    role="navigation"
    aria-label="main navigation"
  >
    <div class="container">
      <div class="navbar-brand">
        <nuxt-link class="navbar-item" to="/">
          <Logo class="header-logo" />
          <div class="logo-text">
            <h1 class="logo-title">Jasmine Music Theory</h1>
            <p class="logo-subtitle">Music With an Impact</p>
          </div>
        </nuxt-link>

        <a
          role="button"
          class="navbar-burger burger"
          aria-label="menu"
          aria-expanded="false"
          data-target="mobileMenu"
          @click="mobile_menu = !mobile_menu"
        >
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div
        id="mobileMenu"
        class="navbar-menu"
        :class="{ 'is-active': mobile_menu }"
      >
        <div class="navbar-end">
          <nuxt-link to="/about" class="navbar-item">
            About
          </nuxt-link>
          <nuxt-link to="/service-pages" class="navbar-item">
            Services
          </nuxt-link>
          <nuxt-link to="/contact" class="navbar-item">
            Contact
          </nuxt-link>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import Logo from "~/assets/icons/Logo.svg";
export default {
  name: "Header",
  components: {
    Logo
  },
  data() {
    return {
      mobile_menu: false
    };
  }
};
</script>
