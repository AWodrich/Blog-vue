<template>
    <div class="btn">
        <a :href="href" class="btn__btn-primary btn__btn-primary--white btn__btn-primary--animated">{{ btnText }}</a>
    </div>
</template>

<script>
export default {
    data() {
        return {
            href: '#' + this.btnText
        }
    },
    props:['btnText']

}
</script>

<style lang="scss">
    @import "../sass/main";
</style>
