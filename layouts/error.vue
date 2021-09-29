<template>
  <v-app>
    <v-main class="white">
      <v-container class="d-flex flex-column justify-center align-center">
        <v-img
          v-if="error.statusCode === 404"
          :src="errorImg"
          class="mx-auto"
          max-width="50%"
          contain
        ></v-img>

        <h1 v-else>
          {{ otherError }}
        </h1>
        <v-btn class="mt-6" to="/"> Back to Home</v-btn>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import errorImg from '@/assets/404-error.jpg'
export default {
  layout: 'empty',
  props: {
    error: {
      type: Object,
      default: null,
    },
  },
  data() {
    return {
      errorImg,
      pageNotFound: '404 Not Found',
      otherError: 'An error occurred',
    }
  },
  head() {
    const title =
      this.error.statusCode === 404 ? this.pageNotFound : this.otherError
    return {
      title,
    }
  },
}
</script>

<style scoped>
h1 {
  font-size: 20px;
}
</style>
