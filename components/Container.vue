<template>
  <div class="container">
    <div class="row d-flex justify-content-center">
      <div class="p-5">
        <b-nav class="navigator">
          <h4><Logo /></h4>
          <h4>
            <NuxtLink to="/home">Home</NuxtLink>
          </h4>
          <h4>
            <NuxtLink to="/sobre">Sobre</NuxtLink>
          </h4>
        </b-nav>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NuxtContainer',
}
</script>
