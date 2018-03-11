<template>
    <div>
        <div class="image-composition" v-for="(image, index) in imageList">
            <img class="image-composition__photo" :src="image" alt="image-composition" @mouseover="hoverover(index)" @mouseout="hoverout(index)" :class="{ hovered: index == hovered }" />
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            hovered: null
        }
    },
    props: ['imageList'],
    methods: {
        hoverover(index) {
            this.hovered = index;
        },
        hoverout(index) {
            this.hovered = null
        }
    }

}
</script>

<style lang="scss">
    @import "../sass/main";
</style>
