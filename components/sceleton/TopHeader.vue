<template>
  <div class="border-bottom p-2">
    <div class="text-top-head d-flex justify-content-between container-xxl align-items-center">
      <div class="d-flex align-items-center">
        <button class="btn-font btn btn-sm rounded-lg btn-primary-lvl1 p-0 pr-2 pl-2">
          COVID-19 UPDATE
        </button>
        <div class="ml-2">
          We are open with limited hours and staff.
        </div>
      </div>
      <div class="d-flex justify-content-end right-top-header">
        <a target="_blank" href="https://google.com/maps" class="align-items-center d-flex mr-2">
          <i class="fas fa-map-marker-alt" />
          <div class="ml-1">
            Store Location
          </div>
        </a>
        <div class="divider">
          |
        </div>
        <a target="_blank" href="tel:+79656374254" class="align-items-center d-flex ml-2">
          <i class="fas fa-phone" />
          <div class="ml-1">
            +7 (965) - 637 - 4254
          </div>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TopHeader',
  components: {}
}
</script>

<style lang="scss">

.divider{
  font-size: 18px;
  color: #ABABAB;
}
.right-top-header {
  >a:hover{
    color: black;
    -webkit-transition: all 300ms cubic-bezier(.42, 0, 1, 1);
    -moz-transition: all 300ms cubic-bezier(.42, 0, 1, 1);
  }
  > a {
    transition-property: color;
    -webkit-transition: all 300ms cubic-bezier(.42, 0, 1, 1);
    -moz-transition: all 300ms cubic-bezier(.42, 0, 1, 1);
    color: #ABABAB;
    text-decoration: none;
  }

  font-weight: 500;
  line-height: 1;
}

.text-top-head {
  font-size: 14px;
  font-weight: 400;
  line-height: 1.78;
  color: #696969;
}

.btn-font:hover{
  background-color: #E4573D;
  border-color: #E4573D;
  -webkit-transition: all 300ms cubic-bezier(.42, 0, 1, 1);
  -moz-transition: all 300ms cubic-bezier(.42, 0, 1, 1);
}

.btn-font {
  -webkit-transition: all 300ms cubic-bezier(.42, 0, 1, 1);
  -moz-transition: all 300ms cubic-bezier(.42, 0, 1, 1);
  font-size: 14px;
  line-height: 1.78;
  font-weight: 500;
}

</style>
