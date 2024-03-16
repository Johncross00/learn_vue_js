<template>
    <div>
        <h1>Enfant</h1>
        <h2>{{ name }}</h2>
        <h2>{{ userchild.email }}</h2>
        <button v-on:click="passData()" >Call</button>
    </div>
</template>

<script>
export default{
    name: "childComp",
    props: {
        name: String,
        userchild: Object,
        passData: Function
    }
}
</script>