<template>
  <div class="karmen-nav">
    <div class="section left">
    </div>
    <div class="section right">
      <span>
        <select class="karmen-lang">
          <option>Türkçe</option>
          <option>English</option>
        </select>
      </span>
    </div>
  </div>

  <video class="karmen-video" src="/assets/flowers.mp4" controls="false" autoplay muted loop/>

  <div class="karmen-video-overlay"></div>

  <div class="karmen-content">
    <div class="karmen-col">
      <KarmenSection
        link="http://guidancyeventsolutions.com" 
        image="/assets/guidancy-logo.png"
        title="Guidanc'y"
        subtitle="Event Solutions & Consultancy"
      />
    </div>
    <div class="karmen-col">
      <KarmenSection
        link="http://gingeristanbul.com"
        image="/assets/gingeristanbul-logo.png"
        title="Ginger"
        subtitle="Patisserie & Catering"
      />
    </div>
  </div>
</template>

<script>

import KarmenSection from './components/KarmenSection.vue';

export default {
  name: 'App',
  components: {
    KarmenSection
  },
  mounted(){
    
  }
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@400&display=swap');

body,html{
  /*background-color:rgb(248,247,239);*/
  height:100%;
  margin:0;
  padding:0;
}

#app{
  height:100%;
}

.karmen-content{
  height:100%;
  display:flex;
  justify-content: center;
  font-family: 'Raleway', sans-serif;
}

.karmen-col{
  display:flex;
  align-self: center;
  margin:32px;
}

.karmen-nav{
  position:fixed;
  left:0;
  right:0;
  /*background-color:rgba(228,227,219,0.9);*/
  padding:6px 64px;
}

.karmen-nav .section{
}

.karmen-nav .section.left{
  float:left;
}

.karmen-nav .section.right{
  float:right;
}

.karmen-lang{
  text-align:left;
  padding:6px 12px;
  border:none;
  border-radius:4px;
  margin:0px;
}

.karmen-video{
  position:fixed;
  top:50%;
  left:50%;
  transform:translate(-50%,-50%);
  z-index:-1000;
  background-color:rgba(0,0,0,0.5)
}

.karmen-video-overlay{
  position:fixed;
  top:0;
  left:0;
  right:0;
  bottom:0;
  z-index:-999;
  background-color:rgba(228,227,219,0.6);
}
</style>
