<template>
  <section class="home">
    <div class="home-hero">
      <div class="columns  is-centered">
        <div class="column is-half has-text-centered">
          <div class="hero-text">
            <Logo class="hero-logo" />
            <h1 class="hero-title">Jasmine Music Theory</h1>
            <p class="hero-subtitle">Music With an Impact</p>
          </div>
        </div>
      </div>
    </div>
    <div class="section home-section">
      <div class="container">
        <h2 class="title">What is Music Therapy?</h2>
        <div class="columns">
          <div class="column is-7">
            <div class="text-indent">
              <p>
                It’s universally and intuitively understood that “music is good
                for you.”
              </p>
              <p>
                People all around the world harness the power of music every day
                to navigate heartbreak, motivate themselves during a workout,
                celebrate with friends, or relieve stress, as just a few simple
                examples.
              </p>
              <p>
                Music therapy takes this “music is good for you” concept and
                applies it to a wide range of emotional, social, psychological,
                cognitive, spiritual, and physical conditions and challenges. It
                is a clinical, evidence-based practice that uses our inherent
                connection to music in creative, interactive, and unexpected
                ways to achieve some incredible results.
              </p>
            </div>
          </div>
          <div class="column has-text-centered-mobile has-text-right-desktop">
            <img src="~/assets/img/home-piano.jpg" alt />
          </div>
        </div>
      </div>
    </div>
    <div class="has-background-grey-lighter">
      <div class="section home-section two">
        <div class="container">
          <h2 class="title has-text-centered">
            Here are just a few examples of what music therapy can do:
          </h2>
          <div class="columns is-centered">
            <div class="column is-half-desktop ">
              <ul class="list-menu">
                <li>
                  A teen with mental health issues discovers a sense of
                  self-worth and empowerment
                </li>
                <li>A person struggling with addiction remains in recovery</li>
                <li>
                  An individual at the end of life (and their family) have time
                  to experience connection and process emotion
                </li>
                <li>
                  A person with cancer has a reduction in pain, nausea, and
                  stress
                </li>
                <li>
                  An individual with Alzheimer’s is able to sing along to songs
                  from their young adulthood, and engage in music-prompted
                  discussion
                </li>
              </ul>
              <p>
                This is really the tip of the iceberg. Music therapy is used in
                all ages and stages of life, and can be found in schools,
                hospitals, recovery centers, long-term care facilities, and
                hospices, to name a few, often in conjunction with other
                professionals and treatments.
              </p>
              <div class="has-text-centered">
                <nuxt-link to="/contact" class="button is-success"
                  >Schedule a free 30-minute consultation</nuxt-link
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="section home-section">
      <div class="container">
        <h2 class="title">Core Services</h2>
        <div class="columns  is-centered">
          <div class="column is-9-desktop">
            <div class="columns is-multiline is-centered">
              <div class="column is-6-tablet is-4-desktop">
                <div class="card service-card-home">
                  <div class="card-image">
                    <figure class="image is-4by3">
                      <img
                        src="~/assets/img/card-img-1.jpg"
                        alt="Placeholder image"
                      />
                    </figure>
                  </div>
                  <footer class="card-footer">
                    <h3>Adolescents</h3>
                  </footer>
                </div>
              </div>
              <div class="column is-6-tablet is-4-desktop">
                <div class="card service-card-home">
                  <div class="card-image">
                    <figure class="image is-4by3">
                      <img
                        src="~/assets/img/card-img-2.jpg"
                        alt="Placeholder image"
                      />
                    </figure>
                  </div>
                  <footer class="card-footer">
                    <h3>Adults in Mental Health Care</h3>
                  </footer>
                </div>
              </div>
              <div class="column is-6-tablet is-4-desktop">
                <div class="card service-card-home">
                  <div class="card-image">
                    <figure class="image is-4by3">
                      <img
                        src="~/assets/img/card-img-3.jpg"
                        alt="Placeholder image"
                      />
                    </figure>
                  </div>
                  <footer class="card-footer">
                    <h3>Addiction Recovery</h3>
                  </footer>
                </div>
              </div>
              <div class="column is-6-tablet is-4-desktop">
                <div class="card service-card-home">
                  <div class="card-image">
                    <figure class="image is-4by3">
                      <img
                        src="~/assets/img/card-img-4.jpg"
                        alt="Placeholder image"
                      />
                    </figure>
                  </div>
                  <footer class="card-footer">
                    <h3>Adaptive Lessons</h3>
                  </footer>
                </div>
              </div>
              <div class="column is-6-tablet is-4-desktop">
                <div class="card service-card-home">
                  <div class="card-image">
                    <figure class="image is-4by3">
                      <img
                        src="~/assets/img/card-img-5.jpg"
                        alt="Placeholder image"
                      />
                    </figure>
                  </div>
                  <footer class="card-footer">
                    <h3>Assisted Living and Memory Care</h3>
                  </footer>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import Logo from "~/assets/icons/Logo.svg";

export default {
  components: {
    Logo
  }
};
</script>
