<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <h1>Two way binding with multiple input</h1>
    <label for="cross">Cross</label>
    &nbsp;
    <input type="checkbox" id="cross" value="cross" v-model="sports">
    <br>
    <label for="enduro">Enduro</label>
    &nbsp;
    <input type="checkbox" id="enduro" value="enduro" v-model="sports">
    <br>
    <label for="trial">Trial</label>
    &nbsp;
    <input type="checkbox" id="trial" value="trial" v-model="sports">

    <h3>Selected Sports: {{ sports }}</h3>


    Players:     &nbsp;<br>
    <label for="ben">Ben</label>
    <input type="radio" name="players" value="Ben" v-model="players">

    <label for="ben">Dic</label>
    <input type="radio" name="players" value="Dic" v-model="players">
    <h3>Players selected: {{ players }}</h3>
    
</template>

<script>
export default{
    name: "inputBoxes",
    data() {
        return {
            sports: [],
            players: [],
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