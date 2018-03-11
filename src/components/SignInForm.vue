<template>
    <div class="signin-wrapper">
        <form class="signin-wrapper__form">
            <input v-model="firstname" type="" />
            <input v-model="surname" type="text" />
            <input v-model="email" type="email" />
            <button @click="getUserData(firstname, surname, email)">Submit</button>
        </form>
    </div>
</template>

<script>
export default {
    data() {
        return {
            firstname: '',
            surname: '',
            email: ''
        }
    },
    methods: {
        getUserData(first, last, mail) {
            if (!first || !last || !mail) {
                return null
            }
            this.firstname = first
            this.surname = last
            this.email = mail
        }
    }
}
</script>

<style lang="scss">

    @import "../sass/main.scss";

</style>
