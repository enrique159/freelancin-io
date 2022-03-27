<template>
  <div id="header-comp">
    <!-- ------ NAVBAR ------ -->
    <nav class="container">
      <div class="row py-4">
        <div class="col col-3">
          <img class="logo" src="@/assets/logo.svg" alt="" />
        </div>
        <div class="col col-6 nav-menu">
          <div class="d-flex w-100 justify-content-center">
            <a href="#" class="nav-menu-item">
              Services <i class="bi bi-caret-down-fill"></i>
            </a>
            <a href="#" class="nav-menu-item"> About us </a>
            <a href="#" class="nav-menu-item"> Blog </a>
          </div>
        </div>
        <div class="col col-3 nav-buttons">
          <div class="d-flex w-100 justify-content-end">
            <button class="btn button-transparent me-3">
              EN <i class="bi bi-caret-down-fill"></i>
            </button>
            <button class="btn button-primary">Contact us</button>
          </div>
        </div>
      </div>
    </nav>
    <img class="header-hero-img" src="@/assets/img/header_hero_img.png" alt="">
    <!-- -------- CONTENT -------- -->
    <div class="container header-content">
      <div class="row w-100">
        <div class="col col-12 col-lg-6">
          <h1 class="header-content-title">Find & Hire Expert Freelancers</h1>
          <p class="header-content-subtext">
            Work with the best freelance talent from around the world on our 
            secure flexible and cost-effective platform.
          </p>
          <div class="d-flex">
            <button class="btn button-primary me-3">Get Started</button>
            <button class="btn button-primary-border">Learn More</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>
#header-comp {
  width: 100%;
  height: 100vh;
  background-image: url("@/assets/img/bg_header.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

.logo {
  width: 128px;
}

.nav-menu-item {
  color: var(--color-gray-5);
  font-weight: var(--font-regular);
  text-decoration: none;
  padding: 0.5rem 1rem;
}

.header-hero-img {
  position: absolute;
  top: 10%;
  right: 20px;
  width: 55%;
  object-fit: contain;
}

.header-content {
  height: 80%;
  display: flex;
  align-items: center;
  .header-content-title {
    font-size: var(--h1-font-size);
    font-weight: var(--font-heavy);
    color: var(--color-gray-2);
    margin-bottom: 1rem;
  }
  .header-content-subtext {
    width: 70%;
    font-size: var(--h3-font-size);
    font-weight: var(--font-regular);
    color: var(--color-gray-4);
  }
}
@media only screen and (max-width: 768px) {
  #header-comp {
    background-position: 65% 50%;
  }
  .logo {
    min-width: 128px;
  }
  .header-content {
    padding: 0 24px;
    .header-content-title {
      font-size: 2.5rem;
    }
    .header-content-subtext {
      width: 100%;
    }
  }
  .header-hero-img {
    display: none;
  }
  .nav-menu, .nav-buttons {
    visibility: hidden;
  }
}
</style>
