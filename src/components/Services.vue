<template>
  <div id="services-comp">
    <div class="container">
      <div class="row text-center">
        <div class="col col-12">
          <h2 class="services-title">Services</h2>
          <p class="services-subtitle">
            Our support team will get assistance from AI-powered suggestions, 
            making it quicker than ever to handle support requests.
          </p>
        </div>
      </div>
      <div class="d-flex mx-5 mt-5">
        <div class="services-card me-5">
          <img class="mx-4" src="@/assets/img/services_icon_1.svg" alt="">
          <div>
            <h4>Branding Idendity</h4>
            <p class="m-0">
              Our support team will get<br>assistance from AI-powered.
            </p>
          </div>
        </div>
        <div class="services-card">
          <img class="mx-4" src="@/assets/img/services_icon_2.svg" alt="">
          <div>
            <h4>Branding Consult</h4>
            <p class="m-0">
              Our support team will get <br> assistance from AI-powered.
            </p>
          </div>
        </div>
      </div>
      <div class="d-flex justify-content-end mx-5 mt-3">
        <div class="services-card me-5">
          <img class="mx-4" src="@/assets/img/services_icon_3.svg" alt="">
          <div>
            <h4>web development</h4>
            <p class="m-0">
              Our support team will get<br> assistance from AI-powered.
            </p>
          </div>
        </div>
        <div class="services-card">
          <img class="mx-4" src="@/assets/img/services_icon_4.svg" alt="">
          <div>
            <h4>market anlysis</h4>
            <p class="m-0">
              Our support team will get <br> assistance from AI-powered.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Services'
  }
</script>

<style lang="scss" scoped>
#services-comp {
  width: 100%;
  height: 80vh;
  position: relative;
  &::before {
    content: '';
    position: absolute;
    background-image: url('@/assets/img/services_bg_asset.svg');
    background-size: contain;
    background-position: center;
    background-repeat: no-repeat;
    top: 60px;
    left: 5%;
    width: 200px;
    height: 200px;
    z-index: -1;
  }
  &::after {
    content: '';
    position: absolute;
    background-image: url('@/assets/img/services_bg_asset.svg');
    background-size: contain;
    background-position: center;
    background-repeat: no-repeat;
    bottom: 120px;
    right: 5%;
    width: 200px;
    height: 200px;
    z-index: -1;
  }

  .services-title {
    font-size: var(--biggest-font-size);
    font-weight: bold;
    color: var(--color-gray-1);
  }
  .services-subtitle {
    font-size: var(--h3-font-size);
    font-weight: var(--font-regular);
    color: var(--color-gray-4);
    width: 50%;
    margin: 0 auto;
  }

  .services-card {
    background-color: var(--color-white);
    border: 1px solid rgba(239, 239, 239, 0.6);
    box-sizing: border-box;
    box-shadow: 0px 15px 30px rgba(99, 122, 166, 0.08);
    border-radius: 8px;
    padding: 2rem 3rem 2rem 0;
    display: flex;
    img {
      width: 42px;
    }
    h4 {
      text-transform: uppercase;
      font-size: var(--h2-font-size);
      font-weight: var(--font-heavy);
      color: var(--color-gray-2);
    }
  }
}
</style>