<template>
  <nav class="navbar sticky-top justify-content-center">
    <div class="container-fluid d-flex justify-content-center">
      <a class="navbar-brand" href="#">
        <img src="/icon.png" alt="logo" width="64">
      </a>
      <ul class="nav">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Active</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link</a>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
        </li>
      </ul>
      <div class="d-flex">
        <input class="form-control mr-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-success">
          Search
          <svg class="bi" width="32" height="32" fill="currentColor">
            <use xlink:href="node_modules/bootstrap-icons/bootstrap-icons.svg#heart-fill" />
          </svg>
        </button>
      </div>
    </div>
  </nav>
</template>

<script>
export default {}
</script>

<style scoped>

</style>
