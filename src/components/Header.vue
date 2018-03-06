<template>
  <div class="header-wrapper">
      <div class="header-wrapper__primary-text">
          <p>Petition</p>
      </div>
      <div class="navigation-wrapper">
          <p class="navigation-wrapper__item">About us</p>
          <p class="navigation-wrapper__item">Projects</p>
          <p class="navigation-wrapper__item">Map</p>
      </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">

    @import "../sass/vars.scss";
    @import "../sass/mixins.scss";

    .header-wrapper {
        @include style-wrapper;
        @include flex-row;
        @include background-color($secondary-color);

        box-sizing: border-box;
        padding: 1rem;

        &__primary-text {
            @include font-size($primary-size);
            flex: 1;
            text-align: center;
        }
    }

    .navigation-wrapper {
        @include font-size($secondary-size);
        @include flex-row;
        justify-content: flex-end;
        flex: 1;

        &__item {
            margin: 1rem;
        }
    }
    
</style>
