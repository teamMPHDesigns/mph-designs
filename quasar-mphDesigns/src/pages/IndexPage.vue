<template>
  <q-card style="height: 100%; width: 100%;" class="bg-brown-4 q-pa-sm">
    <q-card-section>
      <q-carousel
      v-model="slide"
      transition-prev="slide-down"
      transition-next="slide-up"
      swipeable
      animated
      navigation
      arrows
      class="text-white rounded-borders bg-brown-8"
      style="height:60vh;"
    >
      <q-carousel-slide name="home">
        <q-card class="bg-brown row justify-center">
          <div class="full-width transparent  text-center round-borders" >
          </div>
          <q-card-section style="height: 50vh; width: 40vw;">
            <q-img
              src="~src/assets/home1.jpeg"
              class="rounded-borders"
              :ratio="16/9"
            >
            </q-img>
          </q-card-section>
        </q-card>

      <div class="q-mt-xs text-center">
          wibbly wobbly the description
        </div>
        <div class="q-mt-xs text-center">
          Price abouts $tree.50
        </div>
      </q-carousel-slide>

      <q-carousel-slide name="home2">
        <q-card class="bg-brown row justify-center">
          <div class="full-width transparent  text-center round-borders" >
          </div>
          <q-card-section style="height: 50vh; width: 40vw;">
            <q-img
              src="~src/assets/home2.jpeg"
              class="rounded-borders"
              :ratio="16/9"
            >
            </q-img>
          </q-card-section>
        </q-card>

      <div class="q-mt-xs text-center">
          wibbly wobbly the description
        </div>
        <div class="q-mt-xs text-center">
          Price abouts $tree.50
        </div>
      </q-carousel-slide>

      <q-carousel-slide name="home3">
        <q-card class="bg-brown row justify-center">
          <div class="full-width transparent  text-center round-borders" >
          </div>
          <q-card-section style="height: 50vh; width: 40vw;">
            <q-img
              src="~src/assets/home3.jpeg"
              class="rounded-borders"
              :ratio="16/9"
            >
            </q-img>
          </q-card-section>
        </q-card>

      <div class="q-mt-xs text-center">
          wibbly wobbly the description
        </div>
        <div class="q-mt-xs text-center">
          Price abouts $tree.50
        </div>
      </q-carousel-slide>

    </q-carousel>
    </q-card-section>

    <q-card-actions>
      <q-btn class="col bg-light-blue text-bold">Place an Order</q-btn>
    </q-card-actions>
  </q-card>
</template>

<style scoped>
.my-font {
  font-family: 'Rustic';
}
.woodcarving-website {
  text-align: center;
}

.font-rustic-script {
  font-family: 'Your Rustic Script Font', cursive;
}

.font-woodcut {
  font-family: 'Your Woodcut Font', serif;
}

.font-vintage-display {
  font-family: 'Your Vintage Display Font', cursive;
}

.font-clean-sans-serif {
  font-family: 'Your Clean Sans Serif Font', sans-serif;
}

.font-serif-with-flourishes {
  font-family: 'Your Serif Font with Flourishes', serif;
}

.font-handwritten {
  font-family: 'Your Handwritten Font', cursive;
}

.font-combination {
  font-family: 'Your Combination Font', cursive;
}
</style>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref('home'),
      taco: ref('https://th.bing.com/th/id/R.9df61313bc172f82ed2adc28eea6f309?rik=awgWykoOWKSLBw&pid=ImgRaw&r=0'),
      lorem: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque voluptatem totam, architecto cupiditate officia rerum, error dignissimos praesentium libero ab nemo.'
    }
  }
}
</script>
