<template>
  <div class="container-fluid" id="app">
    <div class="row">
      <ImageSection />
      <InformationSection />
    </div>
  </div>
</template>

<script>

import ImageSection  from './components/ImageSection.vue'
import InformationSection from './components/InformationSection.vue'

export default {
  name: 'app',
  components: {
    ImageSection,
    InformationSection,
  }
}
</script>
