<template>
  <div class="about">
    <h1>This is an about page</h1>
      <vueper-slides
       class="no-shadow"
        ref="vueperslides2"
        :slide-ratio="1 / 8"
        :dragging-distance="50"
        @slide="$refs.vueperslides1 && $refs.vueperslides1.goToSlide($event.currentSlide.index, { emit: false })"
        :visible-slides="3"
        fixed-height="100px"
        :arrows="false"
        :bullets="false">
        <vueper-slide
        v-for="i in 8"
        :key="i"
        @click.native="$refs.vueperslides2 && $refs.vueperslides2.goToSlide(i - 1)">
          <template v-slot:content>
            <div class="vueperslide__content-wrapper" style="font-weight:'bold'">
              <div class="vueperslide__title">{{ i.toString() }}</div>
            </div>
          </template>
        </vueper-slide>
      </vueper-slides>
    <vueper-slides
     class="no-shadow"
        ref="vueperslides1"
        @slide="$refs.vueperslides2 && $refs.vueperslides2.goToSlide($event.currentSlide.index, { emit: false })"
        :slide-ratio="1 / 4"
        :arrows="false"
        :bullets="false">
        <vueper-slide
          v-for="i in 8"
          :key="i"
          :title="i.toString()"
          content="Navigation in sync"
          :style="'background-color: ' + ['#ff5252', '#42b983'][i % 2]" />
      </vueper-slides>

  </div>
</template>

<script>
import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'
export default {
  name:"About",
  components:{
    VueperSlides, VueperSlide
  },
  data: ()=>{

  }
}
</script>
