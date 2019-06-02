<template>
  <div class="columns is-centered">
    <div class="column is-one-third-desktop">
      <div class="card contact-form has-text-left">
        <h2 class="title has-text-centered">Contact Me!</h2>
        <div class="field">
          <label class="label">Name</label>
          <div class="control has-icons-left">
            <input
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
              class="input"
              type="email"
              placeholder="Enter email address"
              value=""
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
              class="textarea"
              placeholder="Enter message"
              required
            ></textarea>
          </div>
        </div>

        <div class="field">
          <div class="control has-text-centered">
            <button class="button is-success">Submit</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactForm",
  data() {
    return {
      date: new Date().getFullYear()
    };
  }
};
</script>
