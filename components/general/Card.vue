<template>
  <div class="rounded p-3 m-2 card-bg flex-fill">
    <div class="card-head-tag">
      Personal
    </div>
    <div class="card-head-name mt-1">
      Temperature Gun
    </div>
    <div class="card-sale">
      $ 35
    </div>
    <button class="mt-3 btn btn-primary rounded-pill pt-2 pb-2 pl-5 pr-5">
      Buy now
    </button>
  </div>
</template>

<script>

export default {
  name: 'Card'
}
</script>

<style scoped lang="scss">
.card-sale{
  font-size: 24px;
  color: #E4573D;
  line-height: 1;
  font-weight: 700;
}

.card-head-name {
  font-size: 24px;
  line-height: 1.5;
  font-weight: 700;
}
.card-bg{
  height: 270px;
  background-color: #f4ede7;
  overflow: hidden;
  background-image: url("https://medizin.thememove.com/wp-content/uploads/2020/04/home-01-product-banner-04.jpg");
  background-repeat: no-repeat;
}

.card-head-tag{
  font-size: 15px;
  text-transform: uppercase;
  color: #333;
}

</style>
