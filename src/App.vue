<template>
  <div class="app-wrapper">
    <Header />
    <About :imageList="imageList"/>
    <hr>
    <SignInForm />
  </div>
</template>

<script>
import Header from './components/Header'
import About from './components/About'
import SignInForm from './components/SignInForm'

import Image from './assets/img-main.jpg'
import img1 from './assets/img-1.jpg'
import img2 from './assets/img-2.jpg'
import img3 from './assets/img-3.jpg'
import img4 from './assets/img-4.jpg'

// import GridTestings from './components/GridTestings'

export default {
    data() {
        return {
            imageSrc: Image,
            imageList: [img1, img2, img3, img4]
        }
    },
    components: {
        Header,
        SignInForm,
        About,
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
