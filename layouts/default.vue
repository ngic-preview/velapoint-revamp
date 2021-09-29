<template>
  <v-app>
    <!-- <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer> -->

    <v-app-bar height="82" color="white" fixed app>
      <v-app-bar-nav-icon
        v-if="$vuetify.breakpoint.sm"
        @click.stop="drawer = !drawer"
      />
      <NuxtLink to="/">
        <v-img max-height="60" contain :src="logo" width="230"></v-img>
      </NuxtLink>

      <v-spacer></v-spacer>

      <v-btn text class="text-none" to="/">Home</v-btn>

      <v-btn text class="text-none mx-1" to="">Get Insured</v-btn>

      <v-btn text class="text-none" to="">About Us</v-btn>

      <v-btn text class="text-none mx-1" to="">Blog</v-btn>

      <div class="d-flex justify-center ml-1">
        <v-btn
          rounded
          color="primary"
          class=""
          :href="`tel:${$store.state.config.phoneNumber}`"
        >
          <v-icon left size="16">mdi-phone</v-icon>
          {{ $store.state.config.phoneNumberFormatted }}
        </v-btn>
      </div>
    </v-app-bar>
    <v-main>
      <Nuxt />
    </v-main>

    <v-footer absolute app color="secondary" dark>
      <v-container class="py-0">
        <v-card color="transparent" flat class="mx-auto">
          <v-card-text class="text-center">
            <v-btn text class="" href="/">Home</v-btn>

            <v-btn text class="" href="">Get Insured</v-btn>

            <v-btn text class="" href="">About Us</v-btn>

            <v-btn text class="" href="">Blog</v-btn>

            <v-btn
              rounded
              color="primary"
              class="ml-2"
              :href="`tel:${$store.state.config.phoneNumber}`"
            >
              <v-icon left size="16">mdi-phone</v-icon>
              {{ $store.state.config.phoneNumberFormatted }}
            </v-btn>
          </v-card-text>

          <v-card-text class="text-justify py-0">
            A website owned by VelaPoint, LLC, markets products underwritten by
            National Health Insurance Company, Integon National Insurance
            Company and Integon Indemnity Corporation. Velapoint, National
            Health Insurance Company, Integon National Insurance Company and
            Integon Indemnity Corporation are all related companies under
            National General Holdings Corp.
          </v-card-text>

          <v-card-text class="text-center py-0">
            <a
              class="text-decoration-none"
              href="https://nghcprivacy.com/ca-notice-at-collection"
              >California Consumer Privacy</a
            >
            | &copy; {{ new Date().getFullYear() }} VelaPoint
          </v-card-text>
        </v-card>
      </v-container>
    </v-footer>
  </v-app>
</template>

<script>
import logo from '@/assets/velapoint-logo-md.png'
export default {
  data() {
    return {
      logo,

      drawer: false,

      /* items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ], */
    }
  },
}
</script>

<style lang="scss">
.v-sheet.v-app-bar.v-toolbar:not(.v-sheet--outlined) {
  box-shadow: 0 2px 30px -1px rgba(85, 85, 85, 0.08),
    0 4px 30px 0 rgba(85, 85, 85, 0.06), 0 1px 30px 0 rgba(85, 85, 85, 0.03) !important;
}

.v-application .elevation-4 {
  box-shadow: 0 2px 30px -1px rgba(85, 85, 85, 0.08),
    0 4px 30px 0 rgba(85, 85, 85, 0.06), 0 1px 30px 0 rgba(85, 85, 85, 0.03) !important;
}
.v-application .elevation-6 {
  box-shadow: 0 3px 30px -1px rgba(85, 85, 85, 0.08),
    0 6px 30px 0 rgba(85, 85, 85, 0.06), 0 1px 30px 0 rgba(85, 85, 85, 0.03) !important;
}

.v-toolbar__content {
  max-width: 1185px;
  margin: auto;
}
</style>
