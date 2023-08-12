<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-blue">
      <div class="row text-h6 q-ma-sm justify-center">
        <q-btn
          flat
          dense
          round
          icon="fas fa-pencil-ruler"
        />

        <q-card flat class="full-width row bg-brown-8 justify-center q-ma-sm rounded-borders col-12">
          <div class="full-width row transparent justify-center text-center round-borders" >
              <q-card-section class="row col-6 q-mb-sm bg-brown-6 rounded-borders">
                <div class="bg-brown-10 col-12 text-h4 text-white" style="border-radius: 20px 20px 0 0; border-top: 5px solid rgb(139, 115, 85);">MPH Designs</div>
                <q-btn class="bg-brown-10 col-12 text-subtitle2 text-white" style="border-radius: 0 0 20px 20px; border-bottom: 5px solid  rgb(139, 115, 85);">210-560-0146</q-btn>
              </q-card-section>
          </div>
        </q-card>

        <div class="col-auto row justify-center">
          <q-btn icon="fab fa-facebook" label="Facebook" class="bg-brown-10 q-ma-sm"></q-btn>
          <q-btn icon="fab fa-pintrest" label="Pintrest" class="bg-brown-10 q-ma-sm"></q-btn>
          <q-btn icon="fab fa-etsy" label="Etsy" class="bg-brown-10 q-ma-sm"></q-btn>
          <q-btn icon="fab fa-instagram" label="Instagram" class="bg-brown-10 q-ma-sm"></q-btn>
          <q-btn icon="fab fa-instagram" label="Email" class="q-ma-sm bg-light-blue-10" target="_blank" href="teammphdesigns@gmail.com"></q-btn>
        </div>

      </div>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer>
      <div>Come see at our next event on August 20th</div>
    </q-footer>
  </q-layout>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'MainLayout',
})
</script>
