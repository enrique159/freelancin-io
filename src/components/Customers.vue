<template>
  <div id="customers-comp">
    <div class="container">
      <div class="row text-center">
        <div class="col col-12">
          <h2 class="customers-title">What our Customers say</h2>
          <p class="customers-subtitle">
            All the Lorem Ipsum generators on the Internet tend to repeat
            predefined chunks.
          </p>
        </div>
      </div>
      <div class="card-stack">
        <div class="card-item"></div>
        <div class="card-item"></div>
        <div class="card-item">
          <img src="@/assets/img/customers_image.png" alt="" />
          <h3>{{ customers.name }}</h3>
          <span>{{ customers.job }}</span>
          <p>{{ customers.comment }}</p>
        </div>
        <button class="button button-back">
          <img src="@/assets/img/arrow_left.svg" alt="" />
        </button>
        <button class="button button-next">
          <img src="@/assets/img/arrow_right.svg" alt="" />
        </button>
      </div>
      <div class="dots">
        <div class="dot"></div>
        <div class="dot"></div>
        <div class="dot"></div>
        <div class="dot"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Customers",
  data() {
    return {
      customers: {
        name: "John Doe",
        job: "Developer",
        comment:
          "“Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.”",
        image: "@/assets/customers_image.png",
      },
    };
  },
};
</script>

<style lang="scss" scoped>
#customers-comp {
  width: 100%;
  height: 90vh;

  .customers-title {
    font-size: var(--biggest-font-size);
    font-weight: bold;
    color: var(--color-gray-1);
  }
  .customers-subtitle {
    font-size: var(--h3-font-size);
    font-weight: var(--font-regular);
    color: var(--color-gray-4);
    width: 100%;
    margin: 0 auto;
  }
}
.card-stack {
  width: 60%;
  height: 380px;
  margin: 40px auto;
  position: relative;

  .card-item {
    position: absolute;
    width: 100%;
    height: 320px;
    background: #ffffff;
    box-shadow: 0px 20px 60px rgba(46, 33, 61, 0.08);
    border-radius: 10px;
    padding: 2rem 4rem;
    text-align: center;
    top: 0;
    left: 0;
    h3 {
      margin: 8px 0 0;
      font-size: 1.8rem;
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
      color: var(--color-gray-5);
      margin: 8px 0;
    }
    img {
      width: 96px;
      aspect-ratio: 1;
      object-fit: cover;
      border-radius: 50%;
    }
    &:nth-child(1) {
      top: 60px;
      width: 80%;
      left: 10%;
    }
    &:nth-child(2) {
      top: 36px;
      width: 90%;
      left: 5%;
    }
    &:nth-child(3) {
      top: 12px;
    }
  }
  .button {
    position: absolute;
    top: 36%;
    cursor: pointer;
    z-index: 10;
    width: 54px;
    height: 54px;
    border-radius: 50%;
    border: 1px solid var(--color-gray-4);
    background-color: transparent;
    transition: var(--transition-fast);
    display: grid;
    place-items: center;
    &:hover {
      background-color: var(--color-gray-6);
    }
  }
  .button-back {
    left: -76px;
  }
  .button-next {
    right: -76px;
  }
}

.dots {
  width: 100%;
  display: flex;
  justify-content: center;
  column-gap: 0.6rem;
  .dot{
    width: 8px;
    height: 8px;
    border-radius: 50%;
    background-color: var(--color-primary);
    opacity: 0.5;
    &:nth-child(1) {
      opacity: 1;
    }
  }

}
</style>