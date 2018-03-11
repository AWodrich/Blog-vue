<template>
    <div class="header">
        <div class="heading-primary">
            <p class="heading-primary--main">LifeHacks</p>
            <p class="heading-primary--sub">Things to put on your bucket list</p>
        </div>
        <Button :btnText="btnText"/>
    </div>
</template>

<script>
import Button from './Button';
export default {
    name: 'Header',
    data () {
        return {
            btnText: 'about'
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
