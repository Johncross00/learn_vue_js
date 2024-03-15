<template>
    <div>
        <h1>Enfant</h1>
        <h2>{{ name }}</h2>
    </div>
</template>

<script>
export default{
    name: "childComp",
    props: {
        name: String
    }
}
</script>