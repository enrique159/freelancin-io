<template>
  <div id="projects-comp">
    <div class="container">
      <div class="row text-center">
        <div class="col col-12">
          <h2 class="projects-title">Our Projects</h2>
          <p class="projects-subtitle">
            We have been providing great flooring solutions service.
          </p>
        </div>
      </div>
      <div class="d-flex justify-content-center py-3 mt-4">
        <button
          class="btn button-option"
          :class="{ 'button-option-active': item.active }"
          v-for="item in options"
          :key="item.id"
          @click="changeOption(item)"
        >
          {{ item.title }}
        </button>
      </div>
      <div class="d-flex justify-content-end mb-4">
        <button class="button-icon me-2">
          <img src="@/assets/img/arrow_left.svg" alt="">
        </button>
        <button class="button-icon">
          <img src="@/assets/img/arrow_right.svg" alt="">
        </button>
      </div>
      <div class="projects-cards">
        <div class="item-card">
          <img src="@/assets/img/projects_img_1.png" alt="">
          <div class="item-card-content">
            <h4 class="card-title">Quarter</h4>
            <span class="card-text">Company Website</span>
          </div>
        </div>
        <div class="item-card">
          <img src="@/assets/img/projects_img_2.png" alt="">
          <div class="item-card-content">
            <h4 class="card-title">Hotelmania</h4>
            <span class="card-text">Company Website</span>
          </div>
        </div>
        <div class="item-card">
          <img src="@/assets/img/projects_img_3.png" alt="">
          <div class="item-card-content">
            <h4 class="card-title">Furnishop</h4>
            <span class="card-text">Company Website</span>
          </div>
        </div>
        <div class="item-card">
          <img src="@/assets/img/projects_img_4.png" alt="">
          <div class="item-card-content">
            <h4 class="card-title">Thrive CBD</h4>
            <span class="card-text">Company Website</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Projects",
  data() {
    return {
      options: [
        {
          id: 1,
          title: "All",
          active: true,
        },
        {
          id: 2,
          title: "Website",
          active: false,
        },
        {
          id: 3,
          title: "Social Media",
          active: false,
        },
        {
          id: 4,
          title: "UI/UX",
          active: false,
        },
        {
          id: 5,
          title: "Market",
          active: false,
        },
      ],
    };
  },
  methods: {
    changeOption(item) {
      this.options.forEach((option) => {
        option.active = false;
      });
      item.active = true;
    },
  },
};
</script>

<style lang="scss" scoped>
#projects-comp {
  width: 100%;
  height: 90vh;

  .projects-title {
    font-size: var(--biggest-font-size);
    font-weight: bold;
    color: var(--color-gray-1);
  }
  .projects-subtitle {
    font-size: var(--h3-font-size);
    font-weight: var(--font-regular);
    color: var(--color-gray-4);
    width: 30%;
    margin: 0 auto;
  }

  .button-option {
    width: 121px;
    background-color: var(--color-gray-6);
    color: var(--color-gray-5);
    border-radius: 1rem;
    padding: 0.3rem 0.6rem;
    font-size: var(--normal-font-size);
    font-weight: var(--font-regular);
    transition: var(--transition-fast);
    margin: 0 12px;
    cursor: pointer;
    &:hover {
      background-color: #eaeaea;
    }
  }
  .button-option-active {
    background-color: var(--color-primary);
    color: var(--color-white);
    &:hover {
      background-color: var(--color-primary);
    }
  }
  .button-icon {
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
  .projects-cards {
    display: flex;
    column-gap: 2rem;
    overflow: hidden;
    height: fit-content;
    .item-card {
      width: 25%;
      aspect-ratio: 4/3;
      position: relative;
      margin-bottom: 24px;
      clip-path: border-box;
      img {
        position: absolute;
        transition: var(--transition-normal);
        top: 0;
        left: 0;
        width: 100%;
        z-index: 0;
      }
      .item-card-content {
        position: absolute;
        bottom: 0;
        left: 0;
        height: 50%;
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
        border-radius: 0 0 0.6rem 0.6rem;
        background: linear-gradient(180deg, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0.58) 89.58%);
        transition: var(--transition-normal);
        padding: 0.6rem;
        cursor: pointer;
        .card-title {
          font-size: var(--normal-font-size);
          font-weight: var(--font-bold);
          color: var(--color-white);
          margin: 0;
        }
        .card-text {
          font-size: var(--small-font-size);
          font-weight: var(--font-regular);
          color: var(--color-white);
          margin: 0;
        }
      }
      &:hover {
        img {
          transform: scale(1.05);
        }
        .item-card-content {
          height: 30%;
        }
      }
    }
  }
}
</style>