<template>
    <div class="header">
        <div class="heading-primary">
            <p class="heading-primary--main">LifeHacks</p>
            <p class="heading-primary--sub">Never stay still</p>
        </div>
        <div class="header__navigation">
            <p class="header__navigation__item">About us</p>
            <p class="header__navigation__item">Projects</p>
            <p class="header__navigation__item">Map</p>
        </div>
        <Button />

    </div>
</template>

<script>
import Button from './Button';
export default {
    name: 'Header',
    data () {
        return {
        }
    },
    components: {
        Button
    }
}
</script>

<style lang="scss">

    @import "../sass/main";

</style>
