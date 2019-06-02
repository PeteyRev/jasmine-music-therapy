<template>
  <section class="about">
    <div class="section">
      <div class="container">
        <h1 class="has-text-dark page-title">
          About
        </h1>

        <div class="columns is-vcentered">
          <div class="column is-7">
            <div class="content-section">
              <h2 class="title">My Mission</h2>
              <div class="text-indent ">
                <p>
                  To encourage healthy, dynamic relationships with self and
                  others.
                </p>
              </div>
            </div>
            <div class="services">
              <div class="content-section">
                <h2 class="title">Meet Kaitlyn</h2>
                <div class="text-indent no-border">
                  <p>
                    I received my Bachelors of Music Education in Music Therapy
                    from the University of Kansas, and completed an internship
                    at Expressive Therapies Utah in the Salt Lake City area. I
                    have worked with a wide variety of needs and populations,
                    including adolescents and adults in mental health treatment,
                    adults and children with special needs, adult oncology,
                    memory care, assisted living, and hospice. I recognize the
                    whole person, encourage self awareness, and believe that
                    with the right support, people can achieve their full
                    potential. I am committed to providing music therapy
                    services that acknowledge each individual’s journey and that
                    provide opportunities for growth and change at any stage of
                    life.
                  </p>
                  <nuxt-link to="/contact" class="button is-success"
                    >Schedule a free 30-minute consultation</nuxt-link
                  >
                </div>
              </div>
            </div>
          </div>
          <div class="column has-text-centered">
            <img src="~/assets/img/about-img.jpg" alt />
          </div>
        </div>
      </div>
    </div>
    <div class="bottom-hero">
      <img src="~/assets/img/about-hero-bg.jpg" alt />
    </div>
  </section>
</template>
<script>
export default {
  name: "About"
};
</script>
