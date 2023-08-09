<template>
  <q-card style="height: 100%; width: 100%; outline: 5px solid lightblue;" class="bg-brown-1 q-pa-sm">
    <q-card-section class="full-width row transparent justify-center text-center round-borders" >
          <div class="col-12 row bg-brown-6 rounded-borders">
            <div class="bg-brown-10 col-12 text-h4 text-white" style="border-radius: 20px 20px 0 0; border-top: 5px solid rgb(139, 115, 85);">MPH Designs</div>
            <q-btn class="bg-brown-10 col-12 text-subtitle2 text-white" style="border-radius: 0 0 20px 20px; border-bottom: 5px solid  rgb(139, 115, 85);">210-210-210</q-btn>
          </div>
    </q-card-section>
    <q-card-section class="justify-center col-12 row">
      <q-btn class="text-black text-center text-subtitle1 bg-light-blue text-bold">MPHDesignTeams@gmail.com</q-btn>
    </q-card-section>
    <q-card-section>
      <q-carousel
      v-model="slide"
      vertical
      transition-prev="slide-down"
      transition-next="slide-up"
      swipeable
      animated
      navigation
      arrows
      class="text-white rounded-borders bg-brown-8"
      style="height: 62vh;"
    >
      <q-carousel-slide name="home">
        <q-img
        src="~src/assets/blueHouseHome.jpeg"
        class="rounded-borders"
      >
      </q-img>
      <div class="q-mt-xs text-center">
          wibbly wobbly the description
        </div>
        <div class="q-mt-xs text-center">
          Price abouts $tree.50
        </div>
      </q-carousel-slide>

      <q-carousel-slide name="tv" class="column no-wrap flex-center">
        <q-icon name="live_tv" size="56px" />
        <div class="q-mt-md text-center">
          squa
        </div>
      </q-carousel-slide>

      <q-carousel-slide name="layers" class="column no-wrap flex-center">
        <q-icon name="layers" size="56px" />
        <div class="q-mt-md text-center">
          squa
        </div>
      </q-carousel-slide>

      <q-carousel-slide name="map" class="column no-wrap flex-center">
        <q-icon name="terrain" size="56px" />
        <div class="q-mt-md text-center">
          squa
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
