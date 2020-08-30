<template>
  <div class="about">
    <PageHero title="Who We Are?"
      >We are a group of highly skilled experts aiming to provide innovation and
      flexibility to your Business.</PageHero
    >
  </div>
</template>

<script>
import PageHero from '~/components/PageHero'
export default {
  components: {
    PageHero,
  },
  data() {
    return {
      title: 'About Us',
      description: 'About Us Meta Descrituion',
    }
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: this.description,
        },
      ],
    }
  },
}
</script>

<style></style>
