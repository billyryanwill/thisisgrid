<template>

        <div class="grid">
            <div class="title">
                <h1>What is CSS Grid?</h1>
                <button v-on:keyup.enter="transition"></button>
            </div>
        </div>
    
</template>

<script>

export default {
  created: function () {
    
  },
  methods: {
    transition: () => {
      console.log(this.$router.push('/'))
    }
  }
}
</script>

<style lang="scss" scoped>
    
    .grid {

        display:grid;
        grid-gap:16px;
        grid-template-columns:repeat(16,1fr);
        grid-template-rows:repeat(auto-fill, 64px);

    }

    .title {

        grid-column-start:3;
        grid-column-end:span 10;
        grid-row-start:6;

    }

</style>