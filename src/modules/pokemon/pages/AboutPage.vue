<template>
    <h1>About Page</h1>
    <hr>
    <h2>{{ name }}</h2>
    <button @click="onChangeName">
        Cambiar nombre 
    </button>
</template>


<script>
export default {
    data() {
        return {
            name: 'David'
        }
    },
    methods: {
        onChangeName() {
            this.name = 'Daniela'
        }
    },
    beforeCreate() {
        console.log('AboutPage - beforeCreate');
    },
    created() {
        console.log('AboutPage - created');
    },
    beforeMount() {
        console.log('AboutPage - beforeMount');
    },
    mounted() {
        console.log('AboutPage - mounted');
    },
    beforeUpdate() {
        console.log('AboutPage - beforeUpdate');
    },
    updated() {
        console.log('AboutPage - updated');
    },
    active() {
        console.log('AboutPage - active');
    },  
    deactivated() {
        console.log('AboutPage - deactivated');
    },
    beforeUnmount() {
        console.log('AboutPage - beforeUnmount');
    },
    unmounted() {
        console.log('AboutPage - unmounted');
    },
    errorCaptured() {
        console.log('AboutPage - errorCaptured');
    },
    renderTracked() {
        console.log('AboutPage - renderTracked');
    },
    renderTriggered() {
        console.log('AboutPage - renderTriggered');
    },
}
</script>