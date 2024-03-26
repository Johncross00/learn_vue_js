<template>
    <div>
        <h1>Main Component</h1>
    </div>
    <teacherComp name="Bruce" />
    <studentComp name="Lee" />
</template>

<script>
import teacherComp from "./teacher.vue";
import studentComp from "./student.vue";

export default{
    name: "mainComp",
    components: {teacherComp, studentComp}
}
</script>