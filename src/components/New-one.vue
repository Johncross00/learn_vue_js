<template>
    <h1>Email: {{ email }}</h1>
    <h1>Mobile: {{ number }}</h1>
    <h1>Name: {{ getName() }}</h1>
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
            getName(){
                return "Carlos"
            },
        },
}
</script>
<style scoped>
h1{
    color: red;
}
</style>