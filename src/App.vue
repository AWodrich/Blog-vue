<template>
  <div class="app-wrapper">
    <Header />
    <Picture :image="imageSrc" />
    <About />
    <SignInForm />
    <!-- <GridTestings /> -->
  </div>
</template>

<script>
import Header from './components/Header'
import Picture from './components/Picture'
import Image from './assets/image.jpg'
import About from './components/About'
import SignInForm from './components/SignInForm'

// import GridTestings from './components/GridTestings'

export default {
    data() {
        return {
            imageSrc: Image
        }
    },
    components: {
        Header,
        Picture,
        SignInForm,
        About,
        // GridTestings
    }
}
</script>

<style lang="scss">

    @import "./sass/main.scss";

    .app-wrapper {
        @include style-wrapper;
        @include flex-col;
        @include background-color($color-primary);
    }
</style>
