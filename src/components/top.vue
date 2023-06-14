<script setup>
import { ref } from 'vue'
</script>
<template>
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
        class="q-pl-lg q-pr-lg q-pb-lg">

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
  </template>
