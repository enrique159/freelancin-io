<template>
  <div id="stats-comp">
    <div class="container py-5">
      <div class="row py-5">
        <div class="col col-4 text-center px-5">
          <img class="stats-img" src="@/assets/img/stats_icon_1.svg" alt="" />
          <h3 class="stats-title">Grow your audience</h3>
          <p class="stats-content">
            Find new customers and build your email list with lead generation ..
          </p>
        </div>
        <div class="col col-4 text-center px-5">
          <img class="stats-img" src="@/assets/img/stats_icon_2.svg" alt="" />
          <h3 class="stats-title">Boost online sales</h3>
          <p class="stats-content">
            Market your ecommerce business and deliver experiences ..
          </p>
        </div>
        <div class="col col-4 text-center px-5">
          <img class="stats-img" src="@/assets/img/stats_icon_3.svg" alt="" />
          <h3 class="stats-title">Sell your knowledge</h3>
          <p class="stats-content">
            Build a following, engage them with your content ..
          </p>
        </div>
      </div>
      <div class="stats-container-blue">
        <h2>Journey of our Success</h2>
        <div class="d-flex justify-content-around w-100">
          <div class="stats-container-bloc">
            <span>85%</span>
            <p>manage communication more efficiently</p>
          </div>
          <div class="stats-container-bloc">
            <span>95%</span>
            <p>improve communication with customers and clients</p>
          </div>
          <div class="stats-container-bloc">
            <span>75%</span>
            <p>average improvement in team efficiency</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Stats",
};
</script>

<style lang="scss" scoped>
#stats-comp {
  height: 100vh;

  .stats-img {
    width: 62px;
  }
  .stats-title {
    margin: 2rem 0 1rem;
    font-size: var(--h2-font-size);
    font-weight: var(--font-medium);
    color: var(--color-gray-2);
  }
  .stats-content {
    width: 70%;
    margin: 0 auto;
    font-size: var(--normal-font-size);
    font-weight: var(--font-regular);
    color: var(--color-gray-4);
  }

  .stats-container-blue {
    width: 86%;
    height: 420px;
    margin: 0 auto;
    background-color: var(--color-primary);
    border-radius: 1.5rem;
    padding: 4.5rem 0 1rem;
    position: relative;
    clip-path: border-box;
    .stats-container-bloc {
      width: fit-content;
    }
    &::after {
      content: '';
      position: absolute;
      top: 20%;
      right: 10%;
      width: 80%;
      height: 120%;
      border-radius: 1rem;
      background: linear-gradient(270.28deg, #2F3290 17.64%, #FFFFFF 87.77%);
      opacity: 0.05;
      transform: rotate(130deg);
    }
    h2 {
      font-size: 3rem;
      font-weight: var(--font-bold);
      color: var(--color-white);
      margin: 0 0 3rem;
      text-align: center;
    }
    span {
      font-size: 4rem;
      font-weight: var(--font-bold);
      text-decoration: underline;
      color: var(--color-white);
      margin: 0 0 3rem;
      text-align: center;
    }
    p {
      width: 180px;
      font-size: var(--normal-font-size);
      font-weight: var(--font-regular);
      color: var(--color-white);
      margin: 0 0 3rem;
    }
  }
}
</style>