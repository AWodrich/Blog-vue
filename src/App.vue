<template>
  <div class="app-wrapper">
    <Header />
    <Picture />
  </div>
</template>

<script>
import Header from './components/Header'
import Picture from './components/Picture'

export default {
    data() {
        return {
            imageSrc: '../assets/image.jpg'
        }
    },
    components: {
        Header,
        Picture
    }
}
</script>

<style lang="scss">

    @import "./sass/vars.scss";
    @import "./sass/mixins.scss";

    .app-wrapper {
        @include style-wrapper;
        @include flex-col;
        @include background-color($primary-color);
    }
</style>
