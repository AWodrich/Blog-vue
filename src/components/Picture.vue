<template>
    <div class="picture">
        <div>
            <img class="picture--rounded picture--medium-sized" :src="image" />
        </div>
    </div>
</template>

<script>

export default {
    props:['image']
}

</script>

<style lang="scss">

    @import "../sass/main.scss";
    
</style>
