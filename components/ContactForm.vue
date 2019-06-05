<template>
  <div class="columns is-centered">
    <div class="column is-8-tablet is-6-desktop is-4-widescreen">
      <div class="card contact-form has-text-left">
        <form @submit="sendForm">
          <h2 class="title has-text-centered">Contact Me!</h2>
          <div class="field">
            <label class="label">Name</label>
            <div class="control has-icons-left">
              <input
                v-model="form.name"
                class="input"
                type="text"
                placeholder="Enter Name"
                required
              />
              <span class="icon is-small is-left">
                <i class="fas fa-user"></i>
              </span>
            </div>
          </div>

          <div class="field">
            <label class="label">Email</label>
            <div class="control has-icons-left has-icons-right">
              <input
                v-model="form.email"
                class="input"
                type="email"
                placeholder="Enter email address"
                required
              />
              <span class="icon is-small is-left">
                <i class="fas fa-envelope"></i>
              </span>
              <!-- <span class="icon is-small is-right">
              <i class="fas fa-exclamation-triangle"></i>
            </span> -->
            </div>
            <!-- <p class="help is-danger">This email is invalid</p> -->
          </div>

          <div class="field">
            <label class="label">Message</label>
            <div class="control has-icons-left">
              <textarea
                v-model="form.message"
                class="textarea"
                placeholder="Enter message"
                required
              ></textarea>
            </div>
          </div>

          <div class="field">
            <div class="control has-text-centered">
              <button
                type="submit"
                class="button is-success"
                :class="{ 'is-loading': form.loading }"
              >
                Submit
              </button>
            </div>
          </div>
        </form>
      </div>
    </div>
    <div
      v-if="this.form.success"
      class="notification is-primary is-fixed-notification"
    >
      <button class="delete"></button>
      <h2 class="title">Message Sent!</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactForm",
  data() {
    return {
      date: new Date().getFullYear(),
      form: {
        name: "",
        email: "",
        message: "",
        loading: false,
        success: false
      }
    };
  },
  methods: {
    async sendForm(e) {
      this.form.loading = true;
      e.preventDefault();
      try {
        const response = await this.$axios.$post(
          "https://formcarry.com/s/fBKIqzlSKNs",
          {
            name: this.form.name,
            email: this.form.email,
            message: this.form.message
          },
          { headers: { Accept: "application/json" } }
        );
        this.form.loading = false;
        this.showResult();
      } catch (err) {
        console.log(err);
        this.form.loading = false;
      }
    },
    showResult() {
      this.form.success = true;
      setTimeout(() => {
        this.form.success = false;
      }, 3000);
    }
  }
};
</script>
