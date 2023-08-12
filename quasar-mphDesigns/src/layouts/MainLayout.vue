<template>
  <q-layout view="lHh Lpr lFf" class="full-height">
    <q-header elevated class="bg-blue">
      <div class="row text-h6 q-ma-sm justify-center">
        <div class="col-12 text-center bg-brown rounded-borders" style="outline: 7px solid rgb(54, 30, 30);">Come see us at our next event on August 20th!!!</div>

        <q-card flat class="full-width row bg-brown-8 justify-center q-ma-sm rounded-borders col-12">
          <div class="full-width row transparent justify-center text-center round-borders" >
              <q-card-section class="row col-6 q-mb-sm bg-brown-6 rounded-borders">
                <div class="bg-brown-10 col-12 text-h4 text-white" style="border-radius: 20px 20px 0 0; border-top: 5px solid rgb(139, 115, 85);">MPH Designs</div>
                <q-btn :class="$q.screen.lt.md ?'text-subtitle1' : ''" class="bg-brown-10 col-12 text-h6 text-white" style="border-radius: 0 0 20px 20px; border-bottom: 5px solid  rgb(139, 115, 85);">210-560-0146</q-btn>
              </q-card-section>
          </div>
        </q-card>

        <div class="col-auto row justify-center">
          <q-btn icon="fab fa-facebook" label="Facebook" class="bg-brown-10 q-ma-sm"></q-btn>
          <q-btn icon="fab fa-pinterest" label="Pinteresst" class="bg-brown-10 q-ma-sm"></q-btn>
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
      <div class="col-12"></div>
    </q-footer>
  </q-layout>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'MainLayout',
})
</script>
