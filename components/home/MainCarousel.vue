<template>
  <div v-once id="carouselExampleDark" class="carousel carousel-dark slide" data-ride="carousel">
    <ol class="carousel-indicators d-flex justify-content-center align-items-center">
      <li
        v-for="i in 3"
        :key="i"
        :class="{ active: i-1===0 }"
        data-target="#carouselExampleDark"
        :data-slide-to="i-1"
        class="bg-dark rounded-circle"
      />
    </ol>
    <div class="carousel-inner">
      <div v-for="i in 3" :key="i" :class="{ active: i===1 }" class="bg-light d-flex block-slider carousel-item" data-interval="20000">
        <div class="p-1 row container-xxl d-md-flex align-self-center mr-auto ml-auto">
          <div class="col-6">
            <h5>Only <span>${{ i }}</span></h5>
            <h3>Fast Reading Digital Thermometer for Ear & Forehead</h3>
            <p>In 3 seconds, you'll get the exact number of your body's temperature. Suitable for both baby & adult</p>
            <button class="btn btn-primary rounded-pill pt-2 pb-2 pl-5 pr-5">
              Buy now
            </button>
          </div>
          <div class="col-6">
            <img src="/img/slider/01-image.png" alt="img_prod">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'MainCarousel',
  data () {
    return {}
  },
  mounted () {
  }
}
</script>

<style scoped lang="scss">

.carousel-indicators > li {
  width: 8px;
  height: 8px;
}

.carousel-indicators > li.active {
  width: 12px;
  height: 12px;
}

.block-slider {
  height: 65vh;

  > div > div {

    > h3 {

      color: rgb(51, 51, 51);
      font-size: 48px;
      font-weight: 500;
    }

    > h5 {
      color: rgb(228, 87, 61);
      font-size: 24px;
      font-weight: 400;

      > span {
        font-weight: 700;
      }
    }

    > p {
    }
  }
}

</style>
