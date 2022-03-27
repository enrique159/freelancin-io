<template>
  <div id="features-comp">
    <div class="container py-5">
      <div class="row text-center py-5">
        <div class="col col-12">
          <h2 class="features-title">Our Features</h2>
          <p class="features-subtitle">
            Unleash your creativety with a visual collaboration
            plattorm that enables effective ideation
          </p>
        </div>
      </div>
      <div class="row text-center features-blocs">
        <div class="col col-12 col-md-3">
          <img src="@/assets/img/features_icon_1.svg" alt="">
          <h4>Choosing a Service</h4>
          <p>
            Choosing an accountant that matches your needs
          </p>
        </div>
        <div class="col col-12 col-md-3">
          <img src="@/assets/img/features_icon_2.svg" alt="">
          <h4>Our Clients Say</h4>
          <p>
            Read the reviews from some of our satisfied clients
          </p>
        </div>
        <div class="col col-12 col-md-3">
          <img src="@/assets/img/features_icon_3.svg" alt="">
          <h4>Initial Consultation</h4>
          <p>
            Understanding your accountancy requirements
          </p>
        </div>
        <div class="col col-12 col-md-3">
          <img src="@/assets/img/features_icon_4.svg" alt="">
          <h4>Request a Callback</h4>
          <p>
            Lets talk at a more convenient time for you
          </p>
        </div>
      </div>
      <div class="row text-center py-5">
        <a class="features-link" href="#">Learn More ></a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Features'
}
</script>

<style lang="scss" scoped>
#features-comp {
  width: 100%;
  height: 80vh;

  .features-title {
    font-size: var(--biggest-font-size);
    font-weight: bold;
    color: var(--color-gray-1);
  }
  .features-subtitle {
    font-size: var(--h3-font-size);
    font-weight: var(--font-regular);
    color: var(--color-gray-4);
    width: 40%;
    margin: 0 auto;
  }

  .features-blocs {
    h4 {
      margin: 2rem 0 1rem;
      font-size: var(--h3-font-size);
      font-weight: var(--font-heavy);
      color: var(--color-gray-2);
    }
    p {
      width: 70%;
      margin: 0 auto;
      font-size: var(--normal-font-size);
      font-weight: var(--font-regular);
      color: var(--color-gray-4);
    }
  }
  .features-link {
    text-decoration: underline;
    color: var(--color-primary);
    font-size: var(--h3-font-size);
  }
  @media screen and (max-width: 768px) {
    height: fit-content;
    .features-subtitle { width: 100%; }
    .features-blocs {
      h4 {
        margin: 1rem 0 0.5rem;
      }
      p {
        margin-bottom: 2rem;
      }
    }
  }
}
</style>