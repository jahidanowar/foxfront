<template>
  <div class="content-area-title text-center">
    <!-- <hr class="divider" :style="{ 'margin-bottom': height + 'px' }" /> -->
    <h2>{{ title }}</h2>
  </div>
</template>

<script>
export default {
  name: 'Heading',
  props: {
    title: {
      type: String,
      required: true,
    },
    height: {
      type: Number,
      default: 30,
    },
  },
}
</script>

<style lang="scss">
.divider {
  border: 3px solid #f68c1c;
  margin: 0 auto;
  width: 50px;
}
.content-area-title {
  margin-bottom: 30px;
  h2 {
    line-height: 1.1;
    font-size: 2rem;
  }
}
</style>
