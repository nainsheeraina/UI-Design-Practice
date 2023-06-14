<template>
  <q-page>
    <div class="row bg-primary"></div>
    <div class="col">
      <!-- <div class="row" style="width:1520px;margin-left:0;margin-right:0;text-align:center">
        <div class="q-pa-md" style="width:1520px;margin-left:0;margin-right:0;text-align:center"> -->
    <q-carousel
      animated
      v-model="slide"
      navigation
      infinite
      :autoplay="autoplay"
      arrows
      transition-prev="slide-right"
      transition-next="slide-left"
      @mouseenter="autoplay = false"
      @mouseleave="autoplay = true"

    >
      <q-carousel-slide :name="1" img-src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/06/What-is-HTML.jpg" />
      <q-carousel-slide :name="2" img-src="https://www.chawtechsolutions.com/wp-content/uploads/2020/10/java_binary.jpg" />
      <q-carousel-slide :name="3" img-src="https://www.analyticsinsight.net/wp-content/uploads/2022/07/JavaScript-Trendiest-Programming-Language-Every-Coder-Must-Know-in-2022.jpg" />
      <q-carousel-slide :name="4" img-src="https://media.geeksforgeeks.org/wp-content/cdn-uploads/20230305181456/Python4.png" />
    </q-carousel>
  <!-- </div>

      </div> -->

    </div>
    <div class="row bg-red text-center">
      <h3>Our Top Courses</h3>
    </div>
    <div class="q-pa-md row items-start q-gutter-md text-center">
    <q-card class="my-card" flat bordered>
      <q-img
        src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/06/What-is-HTML.jpg"
        style="height: 200px;"
      />

      <q-card-section>
        <div class="text-overline text-orange-9">Course</div>
        <div class="text-h5 q-mt-sm q-mb-xs">HTML</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>

      <q-card-actions>
        <q-btn flat color="primary" label="ADD TO CART" />
        <q-btn flat color="secondary" label="BUY" />

        <q-space />

        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>

      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>
    <q-card class="my-card" flat bordered>
      <q-img
        src="https://www.chawtechsolutions.com/wp-content/uploads/2020/10/java_binary.jpg"
        style="height: 200px;"
      />

      <q-card-section>
        <div class="text-overline text-orange-9">Course</div>
        <div class="text-h5 q-mt-sm q-mb-xs">JAVA</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>

      <q-card-actions>
        <q-btn flat color="primary" label="ADD TO CART" />
        <q-btn flat color="secondary" label="BUY" />

        <q-space />

        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>

      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>
    <q-card class="my-card" flat bordered>
      <q-img
        src="https://www.analyticsinsight.net/wp-content/uploads/2022/07/JavaScript-Trendiest-Programming-Language-Every-Coder-Must-Know-in-2022.jpg"
        style="height: 200px;"
      />

      <q-card-section>
        <div class="text-overline text-orange-9">Course</div>
        <div class="text-h5 q-mt-sm q-mb-xs">JAVASCRIPT</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>

      <q-card-actions>
        <q-btn flat color="primary" label="ADD TO CARD" />
        <q-btn flat color="secondary" label="BUY" />

        <q-space />

        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>

      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>
    <q-card class="my-card" flat bordered>
      <q-img
        src="https://media.geeksforgeeks.org/wp-content/cdn-uploads/20230305181456/Python4.png"
        style="height: 200px;"
      />

      <q-card-section>
        <div class="text-overline text-orange-9">Course</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Python</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>

      <q-card-actions>
        <q-btn flat color="primary" label="ADD TO CART" />
        <q-btn flat color="secondary" label="BUY" />

        <q-space />

        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>

      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>
  </div>
<div class="row">
  <div>
    <h3>Search Any Course</h3>

  <div class="q-pa-md" style="max-width:800px">
    <div class="q-gutter-md">
      <q-input
        v-model="search"
        debounce="1000"
        filled
        placeholder="Search"

      >
        <template v-slot:append>
          <q-icon name="search" />
        </template>
      </q-input>
    </div>
  </div>
</div>
</div>
<div class="row">
</div>
  </q-page>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref(1),
      autoplay: ref(true),
      expanded: ref(false),
      lorem: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',
      search: ref('')

    }
  }
}
</script>
<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 350px
</style>
