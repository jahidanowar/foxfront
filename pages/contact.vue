<template>
  <div class="contact">
    <PageHero title="Let's Talk"
      >Ready To Grow? <br />
      We look forward to hearing from you</PageHero
    >
    <v-container>
      <v-row>
        <v-col cols="12" md="8" sm="12" xs="12" class="mx-auto">
          <v-form class="pa-5">
            <v-text-field
              name="name"
              label="Full Name"
              solo
              flat
              outlined
              dense
            ></v-text-field>
            <v-text-field
              name="email"
              label="Email ID"
              solo
              flat
              outlined
              dense
            ></v-text-field>
            <v-text-field
              name="phone"
              label="Phone Number"
              solo
              flat
              outlined
              dense
            ></v-text-field>
            <v-textarea
              label="Your Requirements or Message"
              name="message"
              solo
              outlined
              flat
            ></v-textarea>
            <v-btn
              block
              color="primary"
              depressed
              large
              :loading="progress"
              @click="progress = !progress"
              >Submit</v-btn
            >
          </v-form>
        </v-col>
      </v-row>
    </v-container>
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
      title: 'Contact Us',
      progress: false,
    }
  },
  watch: {
    progress() {
      setTimeout(() => {
        this.progress = false
      }, 1000)
    },
  },
}
</script>

<style></style>
