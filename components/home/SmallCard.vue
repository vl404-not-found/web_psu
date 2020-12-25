<template>
  <div class="m-3 d-flex flex-column mr-1 ml-1" style="width: 15.5rem;">
    <span class="text-sm badge bg-danger-lvl-1 flex-shrink-1 mr-auto pt-1 pb-1">
      -26%
    </span>
    <img src="/img/products/antisept.jpg" class="card-img-top" alt="logo">
    <nuxt-link class="text-black-50 text-sm mt-2" to="/shop">
      HOSPITAL EQUIPMENT
    </nuxt-link>
    <nuxt-link class="mt-2 name" to="/shop">
      12-Ply Gauze Sponges
    </nuxt-link>
    <div class="name">
      <span class="text-danger-lvl-1">
        $7.00
      </span>
      <span class="text-decoration-line-through text-black-50">
        $10.00
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SmallCard'
}
</script>

<style scoped lang="scss">
* {
  text-decoration: none;
}
.text-sm:hover{
   color: #4e97fd !important;
}

.text-sm {
  font-size: 13px;
}

.name {
  font-size: 18px;
  color: black;
}

</style>
