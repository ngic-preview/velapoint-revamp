<template>
  <div>
    <v-sheet class="grey lighten-4">
      <v-container class="pt-6">
        <v-row justify="center" align="center">
          <v-col cols="12" sm="7">
            <h4 class="text-lg-h1 text-sm-h4 mb-4">
              A better way to find personalized
              <span class="secondary--text">health insurance</span>
            </h4>
            <p class="text-h6 mb-6">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Commodi
              ex facilis ad atque natus tenetur debitis qui quisquam iure amet
              amet consectetur adipisicing elit.
            </p>
            <v-text-field solo label="Zip code">
              <template #prepend-inner>
                <v-icon large class="mr-1">mdi-map-marker-outline</v-icon>
              </template>
              <template #append>
                <v-btn
                  large
                  height="48"
                  color="primary"
                  class="text-none"
                  style="font-size: 1rem"
                  >Get quotes</v-btn
                >
              </template>
            </v-text-field>
          </v-col>

          <v-col cols="12" sm="5">
            <v-img
              :src="heroImg"
              class="rounded-xl elevation-4"
              max-height="475"
              :aspect-ratio="4024 / 5795"
            ></v-img>
          </v-col>

          <v-col cols="12">
            <v-container class="d-flex align-center px-0 pb-2">
              <v-divider></v-divider>
              <span class="text-overline mx-2">Partners</span>
              <v-divider></v-divider>
            </v-container>
          </v-col>

          <v-col
            v-for="(image, i) in partners"
            :key="i"
            cols="2"
            class="mb-5 px-4"
          >
            <v-img :src="image" class="grayscale-img"></v-img>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>
    <TriangleDivider color="gray" />
    <v-sheet color="white">
      <v-container class="py-4 py-lg-9">
        <div class="text-center">
          <div
            class="text-uppercase font-weight-bold body-2 primary--text mb-2"
          >
            Shop with us
          </div>

          <h2 class="text-h3 text-lg-h2">
            Get the health coverage that's right for you
          </h2>

          <v-responsive max-width="1200" class="mx-auto">
            <div class="text-h6 text-lg-h5 mt-4">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus
              impedit error labore doloremque fugit! Dolor fugit molestiae vero
              quos quisquam nobis, eos debitis magni omnis ea incidunt amet
              voluptate dignissimos!
            </div>
          </v-responsive>
        </div>

        <v-row class="mt-4">
          <v-col cols="12" md="6">
            <div class="d-flex">
              <div class="mr-2">
                <v-sheet class="pa-2 rounded grey lighten-4">
                  <v-icon>mdi-heart-outline</v-icon>
                </v-sheet>
              </div>
              <div>
                <div class="text-h5">Personalized Benefits</div>
                <div class="text-h6 mt-1">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse
                  expedita fugit quam aliquam. Autem assumenda
                </div>
              </div>
            </div>
          </v-col>
          <v-col cols="12" md="6">
            <div class="d-flex">
              <div class="mr-2">
                <v-sheet class="pa-2 rounded grey lighten-4">
                  <v-icon>mdi-heart-outline</v-icon>
                </v-sheet>
              </div>
              <div>
                <div class="text-h5">Fast, Free Quotes</div>
                <div class="text-h6 mt-1">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse
                  expedita fugit quam aliquam. Autem assumenda
                </div>
              </div>
            </div>
          </v-col>
          <v-col cols="12" md="6">
            <div class="d-flex">
              <div class="mr-2">
                <v-sheet class="pa-2 rounded grey lighten-4">
                  <v-icon>mdi-heart-outline</v-icon>
                </v-sheet>
              </div>
              <div>
                <div class="text-h5">Lorem Ipsum</div>
                <div class="text-h6 mt-1">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse
                  expedita fugit quam aliquam. Autem assumenda
                </div>
              </div>
            </div>
          </v-col>
          <v-col cols="12" md="6">
            <div class="d-flex">
              <div class="mr-2">
                <v-sheet class="pa-2 rounded grey lighten-4">
                  <v-icon>mdi-heart-outline</v-icon>
                </v-sheet>
              </div>
              <div>
                <div class="text-h5">Lorem Ipsum</div>
                <div class="text-h6 mt-1">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse
                  expedita fugit quam aliquam. Autem assumenda
                </div>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>

    <!-- <TriangleDivider color="blue" style="transform: rotate(180deg)" /> -->
    <v-sheet color="secondary">
      <v-container class="py-4 py-lg-8">
        <v-row>
          <v-col cols="12" md="6">
            <div
              class="
                text-uppercase
                font-weight-bold
                body-2
                primary--text
                mb-2
                mt-0
              "
            >
              Coverage for all
            </div>

            <h2 class="text-h3 text-lg-h2 white--text">
              Individual and family health insurance plans
            </h2>

            <div class="text-h6 text-lg-h5 mt-5 white--text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus
              impedit error labore doloremque fugit! Dolor fugit molestiae vero
              quos quisquam nobis, eos debitis magni omnis ea incidunt amet
              voluptate dignissimos!
            </div>

            <div class="mt-4">
              <v-btn depressed large color="primary" class="text-none"
                >Shop individual plans</v-btn
              >
            </div>
          </v-col>

          <v-col cols="12" md="6">
            <v-img
              v-col
              :src="productImg1"
              class="elevation-6"
              max-height="400"
              height="100%"
              cover
            />
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>

    <WaveDividerBlue />

    <v-sheet color="white">
      <v-container class="py-4 py-lg-8">
        <v-row>
          <v-col cols="12" md="6">
            <v-img
              v-col
              :src="productImg2"
              class="elevation-6"
              max-height="400"
              height="100%"
              cover
            />
          </v-col>
          <v-col cols="12" md="6" class="pl-4 pl-lg-8">
            <div
              class="
                text-uppercase
                font-weight-bold
                body-2
                primary--text
                mb-2
                mt-0
              "
            >
              Flexible term lengths
            </div>

            <h2 class="text-h3 text-lg-h2">
              Short-term health insurance plans
            </h2>

            <div class="text-h6 text-lg-h5 mt-5">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus
              impedit error labore doloremque fugit! Dolor fugit molestiae vero
              quos quisquam nobis, eos debitis magni omnis ea incidunt amet
              voluptate dignissimos!
            </div>

            <div class="mt-4">
              <v-btn depressed large color="secondary" class="text-none"
                >Shop short-term plans</v-btn
              >
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>

    <WaveDividerWhite />

    <v-sheet color="primary">
      <v-container class="py-4 py-lg-8">
        <v-row>
          <v-col cols="12" md="6">
            <div
              class="
                text-uppercase
                font-weight-bold
                body-2
                secondary--text
                mb-2
                mt-0
              "
            >
              Coverage for all
            </div>

            <h2 class="text-h3 text-lg-h2 white--text">
              Individual and family health insurance plans
            </h2>

            <div class="text-h6 text-lg-h5 white--text mt-5">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus
              impedit error labore doloremque fugit! Dolor fugit molestiae vero
              quos quisquam nobis, eos debitis magni omnis ea incidunt amet
              voluptate dignissimos!
            </div>

            <div class="mt-4">
              <v-btn depressed large light class="text-none"
                >Shop individual plans</v-btn
              >
            </div>
          </v-col>

          <v-col cols="12" md="6">
            <v-img
              v-col
              :src="productImg3"
              class="elevation-6"
              max-height="400"
              height="100%"
              cover
            />
          </v-col>
        </v-row>
      </v-container>
    </v-sheet>

    <v-sheet color="grey lighten-4">
      <v-container class="py-4 py-lg-8">
        <div class="text-center">
          <div
            class="text-uppercase font-weight-bold body-2 primary--text mb-2"
          >
            Shop with confidence
          </div>

          <h2 class="text-h3 text-lg-h2">What our customers are saying</h2>

          <v-responsive max-width="1200" class="mx-auto">
            <div class="text-h6 text-lg-h5 mt-4">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus
              impedit error labore doloremque fugit! Dolor fugit molestiae vero
              quos quisquam nobis, eos debitis magni omnis ea incidunt amet
              voluptate dignissimos!
            </div>
          </v-responsive>
        </div>

        <v-carousel
          hide-delimiter-background
          height="auto"
          hide-delimiters
          continuous
          cycle
          class="mt-4 mt-lg-8"
        >
          <template #prev>
            <v-btn icon round light>
              <v-icon large>mdi-chevron-left</v-icon>
            </v-btn>
          </template>
          <template #next>
            <v-btn icon round light>
              <v-icon large>mdi-chevron-right</v-icon>
            </v-btn>
          </template>
          <v-carousel-item v-for="(testimonial, i) in testimonials" :key="i">
            <v-responsive class="px-8 px-md-10 mx-auto h-full" max-width="1200">
              <div class="d-flex flex-column flex-md-row align-center">
                <div class="mr-md-8 mb-4">
                  <v-avatar height="140" min-width="140" width="140">
                    <v-img :src="testimonial.avatar"></v-img>
                  </v-avatar>
                </div>

                <div>
                  <div class="text-h6 text-lg-h5" style="font-weight: 300">
                    <v-icon color="primary" class="mt-n2 mr-1"
                      >mdi-format-quote-open</v-icon
                    >{{ testimonial.quote
                    }}<v-icon color="primary" class="ml-1"
                      >mdi-format-quote-close</v-icon
                    >
                  </div>
                  <div class="text-body-1 text-lg-h6 mt-2">
                    {{ testimonial.name }}
                  </div>
                  <div class="text-body-1 secondary--text">
                    {{ testimonial.role }}
                  </div>
                </div>
              </div>
            </v-responsive>
          </v-carousel-item>
        </v-carousel>
      </v-container>
    </v-sheet>
  </div>
</template>

<script>
import colors from 'vuetify/lib/util/colors'
import partnerLogo1 from '@/assets/partners/logoipsum-logo-2.svg'
import partnerLogo2 from '@/assets/partners/logoipsum-logo-1.svg'
import partnerLogo3 from '@/assets/partners/logoipsum-logo-10.svg'
import partnerLogo4 from '@/assets/partners/logoipsum-logo-29.svg'
import partnerLogo5 from '@/assets/partners/logoipsum-logo-5.svg'
import partnerLogo6 from '@/assets/partners/logoipsum-logo-9.svg'
import heroImg from '@/assets/happy-family.jpg'
import productImg1 from '@/assets/coast-girl.jpg'
import productImg2 from '@/assets/mountain-man.jpg'
import productImg3 from '@/assets/lake-group.jpg'

import TriangleDivider from '@/components/TriangleDivider.vue'
import WaveDividerBlue from '@/components/WaveDividerBlue.vue'
import WaveDividerWhite from '@/components/WaveDividerWhite.vue'
export default {
  components: { TriangleDivider, WaveDividerBlue, WaveDividerWhite },
  data() {
    return {
      colors,
      partners: [
        partnerLogo1,
        partnerLogo2,
        partnerLogo3,
        partnerLogo4,
        partnerLogo5,
        partnerLogo6,
      ],
      testimonials: [
        {
          avatar: 'https://carbon-ui.indielayer.com/images/team/7.jpeg',
          quote:
            'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nemo ipsa quasi quae itaque soluta sapiente.',
          name: 'Ross Tremathack',
          role: 'CEO LeBusinesses',
        },
        {
          avatar: 'https://carbon-ui.indielayer.com/images/team/3.jpeg',
          quote:
            'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nemo ipsa quasi quae itaque soluta sapiente.',
          name: 'Karyn Barszczewski',
          role: 'Found & CEO Company',
        },
      ],
      heroImg,
      productImg1,
      productImg2,
      productImg3,
    }
  },
}
</script>

<style lang="scss">
.v-text-field.v-text-field--solo .v-input__append-outer {
  margin-top: 0 !important;
}

.grayscale-img {
  filter: grayscale(100%) brightness(2);
  width: 180px;
}
.grayscale-img:hover {
  filter: none;
}

.v-text-field.v-text-field--solo:not(.v-text-field--solo-flat)
  > .v-input__control
  > .v-input__slot {
  height: 70px !important;
}

.v-btn__content {
  font-family: 'Heebo', sans-serif;
}

.v-window__next,
.v-window__prev {
  background: none !important;
}
</style>
