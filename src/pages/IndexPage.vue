<template>
  <q-page class="bg-deep-purple-1">
    <top/>
    <LearningLession/>
    <FeaturedLession/>

  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import top from 'src/components/top.vue';
import LearningLession from 'src/components/LearningLession.vue';
import FeaturedLession from'src/components/FeaturedLession.vue';

export default defineComponent({
    name: "IndexPage",
    components: { LearningLession }
})
</script>
