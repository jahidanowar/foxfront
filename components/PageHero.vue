<template>
  <v-container fluid class="bg1 page-hero">
    <v-container>
      <v-row align="center" justify="center">
        <v-col cols="6">
          <h1 class="page-title">{{ title }}</h1>
          <p class="mt-3 page-description"><slot></slot></p>
        </v-col>
        <v-col cols="6">
          <img :src="image" alt="title" class="featured-image" />
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<script>
export default {
  name: 'PageHero',
  props: {
    title: {
      type: String,
      required: true,
    },
    image: {
      type: String,
      default: '',
    },
  },
}
</script>

<style lang="scss" scoped>
.page-hero {
  padding-top: 5%;
  padding-bottom: 5%;
}
.page-title {
  font-size: 3.5rem;
  line-height: 1.1;
}
.page-description {
  font-size: 1.125rem;
  line-height: 1.5;
}
</style>
>
