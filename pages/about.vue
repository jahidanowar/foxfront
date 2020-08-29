<template>
  <div class="about">
    <PageHero title="Who We Are?"
      >Ready To Grow? <br />
      We look forward to hearing from you</PageHero
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
