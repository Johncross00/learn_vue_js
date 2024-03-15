<template>
    <h1>For Loop</h1>
    <ul>
        <li v-for="result in letters"  :key="result">
            {{ result }}
        </li>
        
    </ul>
    <br>
    <hr>

    <ul>
        <li v-for="chiffre in tag" :key="chiffre">
            Name one is: {{ chiffre.name}} &nbsp; <br>
            age one is: {{ chiffre.age}} &nbsp; <br>
            email one is: {{ chiffre.email}}

        </li>
    </ul>
</template>

<script>
export default{
    name: "forLoop",
    data() {
        return {
            letters: ["A", "B", "C"],
            tag: [{
                name: "GUin",
                age: "50",
                email: "email@example.com"
            }]
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