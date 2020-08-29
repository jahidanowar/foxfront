<template>
  <v-card flat align="center" class="pa-5">
    <v-img :src="image" :width="size"></v-img>
    <h3 primary-title class="text-center">
      {{ title }}
    </h3>
    <p class="pa-5">
      {{ description }}
    </p>
    <v-btn text color="primary" class="text-center">Learn More</v-btn>
  </v-card>
</template>

<script>
export default {
  name: 'Blurb',
  props: {
    size: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
    image: {
      type: String,
      required: true,
    },
    description: {
      type: String,
      required: true,
    },
  },
}
</script>

<style></style>
