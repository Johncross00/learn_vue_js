<template>
    <div>
        <h1>Données Non-Props</h1>
        <h2>{{ info }}</h2>
        <h3 v-bind="$attrs">Lorem ipsum dolor sit amet.</h3>
    </div>
</template>

<script>


export default{
    name: "nonPropsComp",
    props: {
        info: String
    }
}
</script>