<template>
    <div>
        <h1>Données Props</h1>
    </div>
    <nonPropsComp info="Hello World" id="name"/>
</template>

<script>
import nonPropsComp from "./nonprops.vue"

export default{
    name: "propsComp",
    components: {nonPropsComp}
};
</script>