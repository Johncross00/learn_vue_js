<template>
    <div>
        <h1>Teacher Component</h1>
        <h1>Teacher name is {{ name }}</h1>
    </div>
    <button v-on:click="getUsers(userName)">Click Name</button>

</template>

<script>
export default{
    name: "teacherComp",
    props: {
        name: String,
        getUsers: Function
    },
    data() {
        return {
            userName: "Clark"
        }
    }
}
</script>