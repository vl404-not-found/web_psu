<template>
  <div>
    <div>
      <MainCarousel />
    </div>
    <div class="mt-3 container-xxl d-flex">
      <Card v-for="i in 3" :key="i" />
    </div>
    <div class="head-title container-xxl mt-5">
      <div>
        Shop by categories
      </div>
      <div class="d-flex">
        <CardCategory v-for="i in 6" :key="i" />
      </div>
    </div>
    <div class="head-title container-xxl mt-5 border border-3 border-primary mb-5">
      <div class="ml-2 block-title-overflow bg-white">
        Daily Deal Of The Day <span class="ml-2 bg-danger-lvl-1 text-white pl-4 p-1 pr-4 rounded-pill">
          End in: 23 : 59 : 59
        </span>
      </div>
      <div class="d-flex flex-wrap justify-content-between">
        <BigCard v-for="i in 5" :key="i" />
      </div>
    </div>
    <div class="container-xxl">
      <div class="row">
        <div class="col-8">
          <Card />
        </div>
        <div class="col-4">
          <Card />
        </div>
      </div>
    </div>
    <div class="head-title container-xxl mt-5">
      <div>
        Best selling items
      </div>
      <div class="row">
        <SmallCard v-for="i in 10" :key="i" />
      </div>
    </div>
    <div class="bg-light mt-5">
      <div class="head-title container-xxl pt-5 pb-5">
        <div>
          Shop by brands
        </div>
        <div class="d-flex flex-wrap">
          <nuxt-link v-for="i in 12" :key="i" to="/" class="m-4">
            <img src="/img/brands/pagemed.png" alt="partner_logo">
          </nuxt-link>
        </div>
      </div>
    </div>
    <div class="head-title container-xxl mt-5">
      <div>
        From our Blog
      </div>
      <div class="row mt-3">
        <div class="col-6">
          <div v-for="i in 2" :key="i" class="d-flex mt-2">
            <div class="position-relative">
              <img src="/img/other/person.jpg" width="300" alt="thumbnail">
              <div class="position-absolute badge bg-primary text-uppercase pt-2 pb-2">
                Hot News
              </div>
            </div>
            <div class="ml-3 mt-4 card-text-blog">
              <div class="text-muted">
                <i class="fa fa-calendar-o" aria-hidden="true" />
                April 21, 2020
              </div>
              Coronavirus latest: at a glance
            </div>
          </div>
        </div>
        <div class="col-6 align-items-center d-flex">
          <div class="bg-light p-5 rounded-lg">
            <div class="content">
              <h3 class="title">
                Great quality!
              </h3>
              <div class="h4">
                This is a great design and I hope that we will create a website with a good signature.
                ThemeMove team is reactive and kind. Thanks for the help so far.
              </div>
              <div class="h5 text-muted">
                Eric from SpaceX.
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="bg-light mt-5">
      <div class="head-title container-xxl">
        <div class="row h6 pointer-bg">
          <div class="col-3 text-center p-3">
            <div class="h4">
              Store location
            </div>
            219 Amara Fort Apt. 394
          </div>
          <div class="col-3 text-center p-3">
            <div class="h4">
              Work inquiries
            </div>
            hello@medizin.com
          </div>
          <div class="col-3 text-center p-3">
            <div class="h4">
              Call us
            </div>
            +7(965)637-42-54
          </div>
          <div class="col-3 text-center p-3">
            <div class="h4">
              Open hours
            </div>
            Mon-Sat : 08.00 - 18.00
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import MainCarousel from '~/components/home/MainCarousel'
import Card from '~/components/general/Card'
import CardCategory from '~/components/general/CardCategory'
import BigCard from '~/components/home/BigCard'
import SmallCard from '~/components/home/SmallCard'

export default {
  components: {
    BigCard,
    SmallCard,
    CardCategory,
    MainCarousel,
    Card
  },
  layout: 'main'
}
</script>

<style lang="scss">
.pointer-bg>*:hover {
  background-color: white !important;
}
.card-text-blog {
  font-size: 20px;
}

.badge {
  font-size: 14px;
  font-weight: 500;
  left: 10px;
  bottom: 10px;
}

.block-title-overflow {
  width: 42%;
  margin-top: -22px;

  span {
    font-size: 20px;
  }
}

.head-title {
  font-size: 30px;
  font-weight: 500;
}

</style>
