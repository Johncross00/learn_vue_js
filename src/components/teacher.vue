<template>
    <div>
        <h1>Teacher Component</h1>
        <h1>Teacher name is {{ name }}</h1>
    </div>
</template>

<script>
export default{
    name: "teacherComp",
    props: {
        name: String
    }
}
</script>