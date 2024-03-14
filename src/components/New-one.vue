<template>
    <h1>Email: {{ email }}</h1>
    <h1>Mobile: {{ number }}</h1>
    <h1>Name: {{ getName("Scouuu") }}</h1>
    <!-- <h2>Email: {{ getData().email }}</h2>
    <h2>Mobile: {{ getData().number }}</h2> -->
    <button v-on:dblclick="getDaata('Hello')">Click here</button>
</template>

<script>
export default{
    name: "PAGES",
    data() {
        return {
            email: "abcd@gmail.com",
            number: "06000000",
        };
    },
    methods: {
            getName(name){
                return name;
            },
            getData(){
                return {
                    email: this.email,
                    number : this.number,
                };
            },
            getDaata(data) {
                alert (data);
            }
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
</style>