<template>
  <section class="section-about">
      <div id="about" class="section-about--centered">
          <h2 class="heading-secondary">
              The Bucket List
          </h2>
      </div>
      <div class="section-about__content-wrapper">
          <div class="col-1-of-2">
              <h3 class="heading-tertiary">What is a Bucket List?</h3>
              <p class="paragraph">If you haven’t heard about the term “bucket list”, it is a list of all the goals you want to achieve, dreams you want to fulfill and life experiences you desire to experience before you die.</p>
              <h3 class="heading-tertiary">Why create a Bucket List?</h3>
              <p class="paragraph">The whole point of creating your list is to maximize every moment of our existence and live our life to the fullest. It’s a reminder of all the things we want to achieve in our time here, so that instead of pandering our time in pointless activities, we are directing it fully toward what matters to us.</p>
          </div>
          <div class="col-1-of-2">
              <ImageComposition :imageList="imageList"/>
          </div>
      </div>
      <div class="section-about__content-wrapper__link">
          <a href="#more" class=btn-text>More &rarr;</a>
      </div>
  </section>
</template>

<script>
import ImageComposition from './ImageComposition'

export default {
    props:['imageList'],
    components: {
        ImageComposition
    }
}
</script>

<style lang="scss">
    @import "../sass/main";
</style>
