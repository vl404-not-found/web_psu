<template>
  <div v-scroll="handleScroll" class="sticky-top top-head-container bg-white">
    <TopHeader />
    <div class="p-2 pt-4 pb-4">
      <div class="d-flex justify-content-between container-xxl align-items-center">
        <div>
          <img class="logo-header" src="~/static/img/logo/dark-logo.png" alt="logo">
        </div>
        <div class="ml-3">
          <ul class="nav mt-1">
            <li class="nav-item">
              <nuxt-link active-class="active" class="nav-link" aria-current="page" exact to="/">
                Home
              </nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link active-class="active" class="nav-link" aria-current="page" to="/products">
                Shop
              </nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link active-class="active" class="nav-link" aria-current="page" exact to="/about">
                About us
              </nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link active-class="active" class="nav-link" aria-current="page" exact to="/contact">
                Contact
              </nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link active-class="active" class="nav-link" aria-current="page" to="/blog">
                Blog
              </nuxt-link>
            </li>
          </ul>
        </div>
        <div class="ml-auto mr-5 flex-grow-1">
          <form
            onsubmit="search"
            class="search-form border-none bg-light rounded-pill d-flex justify-content-between form-control ml-auto w-50 pt-2 pb-2"
          >
            <label class="d-none" for="search-menu" />
            <input id="search-menu" type="text" class="bg-light" placeholder="Search for items...">
            <button type="submit" class="text-black-50 btn p-0 m-0 align-self-end">
              <i class="fas fa-search" />
            </button>
          </form>
        </div>
        <div class="d-flex menu-icons justify-content-around">
          <i class="far fa-heart mr-3" />
          <i class="fas fa-shopping-bag mr-3" />
          <i class="far fa-user mr-3" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TopHeader from '~/components/sceleton/TopHeader'

export default {
  components: { TopHeader },
  methods: {
    search () {
      return 0
    },
    handleScroll (evt, el) {
      if (window.scrollY > 10) {
        el.className = 'shadow sticky-top top-head-container bg-white'
        el.setAttribute(
          'style',
          'opacity: 1; transform: translate3d(0, -43px, 0)'
        )
      } else {
        el.className = 'sticky-top top-head-container bg-white'
        el.setAttribute(
          'style',
          'opacity: 1; transform: translate3d(0, 0, 0)'
        )
      }
    }
  }
}
</script>

<style scoped lang="scss">
.menu-icons{
  :hover{
    color: #4e97fd;
    transition: all 0.2s linear;
  }
  transition: all 0.2s linear;
  color: #333;
  font-weight: 400;
  font-size: 20px;
}
.search-form:hover {
  border-color: blue;
}

.search-form>input {
  outline:0 #0000!important;
  border:0 solid #0000!important;
  :focus {outline:none !important;}
  :active {outline:none !important;}
  ::-moz-focus-inner {border:0 !important;}
}

.top-head-container {
  transition: 0.5s all cubic-bezier(0.39, 0.575, 0.565, 1);
}

ul.nav > * {
  :hover {
    color: #4e97fd;
  }

  > * {
    color: #b59b9b;
    font-size: 16px;
    font-weight: 500;
    line-height: 1.4;
  }
}

.active {
  color: #4e97fd !important;
}

.logo-header {
  width: 166px;
}

</style>
