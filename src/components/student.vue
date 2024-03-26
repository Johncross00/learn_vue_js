<template>
    <div>
        <h1>Student Component</h1>
        <h1>Student Name is {{ name }}</h1>
    </div>
</template>

<script>
export default{
    name: "studentComp",
    props: {
        name: String
    }
}
</script>