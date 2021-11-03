<template>
    <div>
        <h1 class="hi">how are you</h1>
        <h2 v-bind:style="{color:'magenta'}">i am fine</h2>
        <h3 v-bind:class="{arrayclass}">class binding with array</h3>
        <h3 v-bind:class="{display:show}">class binding</h3>
    </div>
</template>

<script>
    export default {
        name:'ruman',
        data() {
            return {
                arrayclass: 'arrayclass',
                show:true
            }
        },
    }
</script>
<style scoped>
.hi{
    color:brown
}
.arrayclass{
    background-color: cadetblue;
}
.display{
    background-color: chartreuse;
}
</style>