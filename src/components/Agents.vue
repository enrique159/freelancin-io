<template>
  <div id="agents-comp">
    <div class="container py-5">
      <div class="row text-center pt-5">
        <div class="col col-12">
          <h2 class="agents-title">Our Featured Agents</h2>
          <p class="agents-subtitle">
            Meet our amazing team members
          </p>
        </div>
      </div>
      <div class="w-75" style="margin: 0 auto;">
        <div class="row pt-3">
          <div class="col col-4">
            <div class="agent-card">
              <div class="d-flex justify-content-between mb-2">
                <img src="@/assets/img/star.svg" alt="" />
                <img src="@/assets/img/threedots.svg" alt="" />
              </div>
              <img src="@/assets/img/agents_img_1.png" alt="" class="mb-3" />
              <h3>Alison Kiara</h3>
              <span>Michigan, TX</span>
              <p>989-653-2986</p>
              <a href="#">alisonkiara@hommy.com</a>
            </div>
          </div>
          <div class="col col-4">
            <div class="agent-card ac-2">
              <div class="d-flex justify-content-between mb-2">
                <img src="@/assets/img/star.svg" alt="" />
                <img src="@/assets/img/threedots.svg" alt="" />
              </div>
              <img src="@/assets/img/agents_img_2.png" alt="" class="mb-3" />
              <h3>Alison Kiara</h3>
              <span>Michigan, TX</span>
              <p>989-653-2986</p>
              <a href="#">alisonkiara@hommy.com</a>
            </div>
          </div>
          <div class="col col-4">
            <div class="agent-card ac-3">
              <div class="d-flex justify-content-between mb-2">
                <img src="@/assets/img/star.svg" alt="" />
                <img src="@/assets/img/threedots.svg" alt="" />
              </div>
              <img src="@/assets/img/agents_img_3.png" alt="" class="mb-3" />
              <h3>Alison Kiara</h3>
              <span>Michigan, TX</span>
              <p>989-653-2986</p>
              <a href="#">alisonkiara@hommy.com</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Agents",
};
</script>

<style lang="scss" scoped>
#agents-comp {
  width: 100%;
  height: 100vh;
  background-color: var(--color-aqua);
  position: relative;
  &::before {
    content: '';
    position: absolute;
    background-image: url('@/assets/img/agents_bg_asset.svg');
    background-size: contain;
    background-position: center;
    background-repeat: no-repeat;
    top: 120px;
    right: 5%;
    width: 200px;
    height: 200px;
    z-index: 0;
  }
  .agents-title {
    font-size: var(--biggest-font-size);
    font-weight: bold;
    color: var(--color-gray-1);
  }
  .agents-subtitle {
    font-size: var(--h3-font-size);
    font-weight: var(--font-regular);
    color: var(--color-gray-4);
    width: 100%;
    margin: 0 auto;
  }
  .agent-card {
    background-color: white;
    width: 100%;
    height: 360px;
    margin: 0 auto;
    border: 1px solid #f6fbfd;
    box-sizing: border-box;
    box-shadow: 0px 20px 50px rgba(198, 217, 225, 0.3);
    border-radius: 5px;
    padding: 2rem;
    text-align: center;
    position: relative;
    z-index: 10;
    h3 {
      margin: 0;
      font-size: 1.5rem;
      font-weight: var(--font-heavy);
      color: var(--color-gray-1);
    }
    span {
      font-size: var(--normal-font-size);
      font-weight: var(--font-medium);
      color: var(--color-gray-5);
    }
    p {
      font-size: var(--normal-font-size);
      font-weight: var(--font-regular);
      color: var(--color-gray-2);
      margin: 24px 0 0;
    }
  }
  .ac-2 {
    margin-top: 2rem;
  }
  .ac-3 {
    margin-top: 4rem;
  }
}
</style>