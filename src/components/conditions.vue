<template>
    <h1 v-if="display" >IF condition</h1>
    <h1 v-else >Else condition</h1>
    <button v-on:click="display = !display">Change</button>
</template>

<script>
export default{
    name: "conditionComp",
    data() {
        return {
            display: false
        };
    },
    
}
</script>
<style scoped>
h1{
    color: greenyellow;
}

h2{
    color: rgb(47, 137, 255);
}

h3{
    color: orange;
}
</style>