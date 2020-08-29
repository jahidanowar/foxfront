<template>
  <v-app id="inspire">
    <Appbar />
    <v-main>
      <Nuxt />
    </v-main>
    <PageFooter />
  </v-app>
</template>

<script>
import Appbar from '~/components/Appbar'
import PageFooter from '~/components/PageFooter'

export default {
  components: {
    Appbar,
    PageFooter,
  },
}
</script>

<style></style>
