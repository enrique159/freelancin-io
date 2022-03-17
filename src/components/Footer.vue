<template>
  <div id="footer-comp">
    <div class="container">
      <div class="row">
        <h1 class="footer-title">
          People who are<br />ready took these courses!
        </h1>
      </div>
      <div class="row pb-5">
        <button class="footer-button">Schedule Appointment</button>
      </div>
      <div class="row pt-5 footer-info">
        <div class="col col-3">
          <img src="@/assets/logo_white.svg" class="mb-5">
          <p>
            Crechterwoord K12 182 DK <br> Alknjkcb, All Rights Reserved
          </p>
        </div>
        <div class="col col-3">
          <p class="link-title">Links</p>
          <ul>
            <li>
              <span>Overons</span>
            </li>
            <li>
              <span>Social Media</span>
            </li>
            <li>
              <span>Counters</span>
            </li>
            <li>
              <span>Contact</span>
            </li>
          </ul>
        </div>
        <div class="col col-3">
          <p class="link-title">Company</p>
          <ul>
            <li>
              <span>Terms & Conditions</span>
            </li>
            <li>
              <span>Privacy Policy</span>
            </li>
            <li>
              <span>Contact</span>
            </li>
          </ul>
        </div>
        <div class="col col-3">
          <p class="link-title">Get in touch</p>
          <ul>
            <li>
              <span>Crechterwoord K12 <br> 182 DK Alknjkcb</span>
            </li>
            <li>
              <span>085-132567</span>
            </li>
            <li>
              <span>info@lobar.net</span>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
#footer-comp {
  width: 100%;
  height: 100vh;
  background-color: var(--color-primary);
  position: relative;
  clip-path: border-box;
  overflow: hidden;

  &::after {
    content: '';
    position: absolute;
    top: -360px;
    right: -200px;
    width: 400px;
    height: 800px;
    border-radius: 1rem;
    background: #0D5FD8;
    opacity: 1;
    transform: rotate(130deg);
    z-index: -1;
  }

  .footer-title {
    font-size: 3rem;
    font-weight: var(--font-bold);
    color: var(--color-white);
    text-align: center;
    margin-top: 120px;
  }
  .footer-button {
    width: 250px;
    margin: 0 auto;
    background-color: var(--color-white);
    color: var(--color-gray-2);
    font-weight: 600;
    padding: 1rem 2rem;
    border-radius: 8px;
    margin-top: 40px;
    cursor: pointer;
  }
  .footer-info {
    color: white;
    .link-title {
      font-weight: var(--font-heavy);
      color: var(--color-white);
      margin: 0;
      margin-bottom: 36px;
    }
    ul {
      list-style: none;
      padding: 0;
      margin: 0;
      li {
        margin-bottom: 18px;
      }
    }
  }
}
</style>