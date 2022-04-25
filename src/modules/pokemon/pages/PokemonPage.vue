<template>
    <h1>Pokemon<span>#{{ id }}</span></h1>
</template>


<script>
export default {
    props: {
        id: {
            type: Number,
            required: true
        }
    },
    data() {
        return {
            // pokemon: null
        }
    },
    created() {
       const {id} = this.$route.params
         this.id = id
    },
}
</script>