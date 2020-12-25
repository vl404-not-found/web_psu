<template>
  <div class="m-3 p-4 rounded flex-column overflow-hidden justify-content-center align-items-center card-cat-bg d-flex text-center">
    <img class="img-cat" src="https://medizin.thememove.com/wp-content/uploads/2020/04/cat-medicine-300x300.jpg" alt="category">
    <div class="name-cat">
      Pharmacy
    </div>
  </div>
</template>

<script>

export default {
  name: 'CardCategory',
  data () {
    return {}
  }
}
</script>

<style scoped lang="scss">

.img-cat{
  width: 130px !important;
}
.name-cat{
  font-size: 18px;
  font-weight: 400;
}
.card-cat-bg{
  >img{
    width: 180px;
  }
  background-color: #f8f8f8;
}
</style>
