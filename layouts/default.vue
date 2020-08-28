<template>
  <v-app id="inspire">
    <Appbar />
    <v-content>
      <Nuxt />
    </v-content>
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
