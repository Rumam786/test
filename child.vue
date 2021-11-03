<template>
    <div>
        <h1>Hello from child component</h1>
        <button v-on:click="updatetitle">update parent</button>
    </div>
</template>

<script>
    export default {
        name:'child',
        methods: {
            updatetitle() {
                this.$emit('changetitle',5)
            }
        },
    }
</script>