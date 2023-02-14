<template>
  <footer class="fixed-bottom p-3">
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <h4><Logo /></h4>
        </div>
        <div class="col-md-6">
          <p class="text-right">Copyright &copy; {{ DateYaer }} iBook</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'NextFooter',
  computed: {
    DateYaer() {
      return new Date().getFullYear()
    },
  },
})
</script>
