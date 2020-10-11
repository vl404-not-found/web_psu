<template>
  <div>
    <TopHeader />
    <div class="p-2 pt-4 pb-3">
      <div class="d-flex justify-content-between container-xxl align-items-center">
        <div>
          <img class="logo-header" src="~/static/img/logo/dark-logo.png" alt="logo">
        </div>
        <div>
          menu
        </div>
        <div>
          search
        </div>
        <div>
          other
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TopHeader from '@/components/sceleton/TopHeader'
export default {
  components: { TopHeader }
}
</script>

<style scoped>

.logo-header{
  width: 166px;
}

</style>
