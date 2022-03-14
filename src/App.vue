<template>
  <div class="karmen-content">
    <div class="karmen-col">
      <KarmenSection :image="'/assets/guidancy-logo.png'"/>
    </div>
    <div class="karmen-col">
      <KarmenSection :image="'/assets/gingeristanbul-logo.png'"/>
    </div>
  </div>
</template>

<script>

import KarmenSection from './components/KarmenSection.vue';

export default {
  name: 'App',
  components: {
    KarmenSection
  }
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@400&display=swap');

.karmen-content{
  display:flex;
  justify-content: center;
  font-family: 'Raleway', sans-serif;
}

.karmen-col{
  display:flex;
  margin:32px;
}

</style>
