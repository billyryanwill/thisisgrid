<template>
  <section class="grid">
    <div>
      <h1>Test</h1>
      <router-link to="what-is">Next</router-link>
    </div>
  </section>
</template>

<script>

export default {
  methods: {
    moveToNextPage (page) {}
  }
}
</script>

<style>
  .grid {

        display:grid;
        grid-template-columns:repeat(16,1fr);
        grid-template-rows:repeat(auto-fill, 64px);

    }
</style>
