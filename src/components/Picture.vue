<template>
    <div class="image-wrapper">
        <div>
            <h1>Image tag</h1>
        </div>
        <!-- <figure src="{image}">Image here:{{this.image}}</figure> -->
    </div>
</template>

<script>

export default {
    name: 'Header',

    data() {
        return {
            image: ''
        }
    },
    props:['image']
}

</script>

<style lang="scss">
    @import "../sass/vars.scss";
    .image-wrapper {
        width: 100%;
        height: 200px;
        border: 2px solid yellow;
        background-color: darken($primary-color, 20%);
    }
</style>
