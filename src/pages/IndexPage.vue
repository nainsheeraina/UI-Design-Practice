<template>
  <q-page class="bg-deep-purple-1">
    <div class="row bg-primary">
      <div class="col">
        <div style=" max-width:650px;margin-left:auto;margin-right:auto;text-align:center">
          <div class="text-h4 text-bold text-white q-mr-xl q-pt-xl q-pb-xl">Learn FullStack Development From Industry Experts!!!!</div>
        <div class="text-h6 text-white q-pl-lg q-pr-lg">Join CodeHelp.io Community Today To Get Started</div>
        <q-input
        color="black"
        bg-color="white"
        filled
        placeholder="Your Email"
        class="q-pl-lg q-pr-lg q-pb-lg"
      >
        <template v-slot:prepend>
          <q-icon name="email" />
        </template>
        <template v-slot:append>
          <q-btn label="Start Learing" color="purple"></q-btn>
        </template>
      </q-input>
        </div>
      </div>
      <div class="col gt-sm">
        <q-img src="src\statics\home-hero-animated.png" style="margin-left:auto;margin-right:auto;display:block; height:450px"></q-img>
      </div>
    </div>
    <div class="row">
      <div class="text-h5 text-bold q-px-sm q-pt-md">Learning Lessions</div>
    </div>
    <div class="row q-pl-lg q-pr-lg q-pb-lg">
      <div class="col-12 col-md">
        <div class="q-pa-md">
    <q-card class="my-card">
      <q-video src="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" />

      <q-card-section>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">by John Doe</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
        eiusmod tempor incididunt ut labore et dolore magna aliqua.
      </q-card-section>
    </q-card>
  </div>
      </div>
      <div class="col-12 col-md">
        <div class="q-pa-md">
    <q-card class="my-card">
      <q-video src="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" />

      <q-card-section>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">by John Doe</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
        eiusmod tempor incididunt ut labore et dolore magna aliqua.
      </q-card-section>
    </q-card>
  </div>
      </div>
      <div class="col-12 col-md">
        <div class="q-pa-md">
    <q-card class="my-card">
      <q-video src="https://www.youtube.com/embed/k3_tw44QsZQ?rel=0" />

      <q-card-section>
        <div class="text-h6">Our Changing Planet</div>
        <div class="text-subtitle2">by John Doe</div>
      </q-card-section>

      <q-card-section class="q-pt-none">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
        eiusmod tempor incididunt ut labore et dolore magna aliqua.
      </q-card-section>
    </q-card>
  </div>
      </div>
    </div>
    <div class="row">
      <div class="text-h5 text-bold q-px-sm q-pt-md">Featured Lessions</div>
    </div>
    <div class="row">
      <div class="col-12 col-md">
        <div class="q-pa-md">
    <q-card class="my-card">
      <div class="row">
        <div class="col-12 col-md-4 q-pa-xs">
          <q-img src="src\statics\248-2480384_web-design-development-web-development-images-png.png"></q-img>
        </div>
        <div class="col-12 col-md-8">
          <div class="text-bold text-h5 text-purple-9 q-pl-md q-pt-sm">Getting Started With FullStack Development!!</div>
        <div class="q-pa-md">In This Course You Will Learn About How to Develop a Website.Learn With The Most Experienced Teachers.</div>
        </div>
      </div>
    </q-card>
  </div>
      </div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage'
})
</script>
