<template>
  <q-card style="height: 100%; width: 100%;" class="bg-brown-4 q-pa-sm">
    <q-card-section>
      <q-carousel
      v-model="slide"

      :transition-prev="$q.screen.lt.md ? 'slide-down' : 'slide-left'"
      :transition-next="$q.screen.lt.md ? 'slide-up' : 'slide-right'"
      swipeable
      autoplay
      infinite
      animated
      navigation
      arrows
      class="text-white rounded-borders bg-brown-8"
      style="height:60vh;"
    >
      <q-carousel-slide v-for="(slide) in this.slideShow" :key="slide.id" :name="slide.id">
        <q-card class="bg-brown row justify-center">
          <div class="full-width transparent text-center rounded-borders" >
          </div>
          <q-card-section :style=" $q.screen.gt.sm ? 'height: 50vh; width: 40vw' : 'height:auto; width:90vw'">
            <q-img
              :src="slide.img"
              class="rounded-borders"
              :ratio=" $q.screen.gt.sm ? 16/9 : 1"
            >
            </q-img>
          </q-card-section>
        </q-card>

      <div class="q-mt-xs text-center text-h6">
        {{ slide.title }}
      </div>
      <div class="q-mt-xs text-center text-bold text-subtitle1">
        {{ slide.desc }}
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
import home1Image from 'assets/home1.jpeg';
import home2Image from 'assets/home2.jpeg';
import home3Image from 'assets/home3.jpeg';

export default {
  data () {
    return {
      slideShow:[
        {
          id:1,
          img: home1Image,
          title: 'From Timber To Treasure and the Skilled hands of A Wood Maker',
          desc: 'MPH Comes To Share Their Art With San Antonio',
        },        {
          id:2,
          img: home2Image,
          title: 'From Timber To Treasure and the Skilled hands of a wood maker',
          desc: 'MPH Comes To Share Their Art With Shertz-Cibolo',
        },        {
          id:3,
          img: home3Image,
          title: 'From Timber To Treasure and the Skilled hands of a wood maker',
          desc: 'MPH Comes To Share Their Art With Shertz-Cibolo',
        },
      ]
    }
  },
  setup () {
    return {
      slide: ref(1),
      taco: ref('https://th.bing.com/th/id/R.9df61313bc172f82ed2adc28eea6f309?rik=awgWykoOWKSLBw&pid=ImgRaw&r=0'),
      lorem: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque voluptatem totam, architecto cupiditate officia rerum, error dignissimos praesentium libero ab nemo.'
    }
  }
}
</script>
