<template>
    <div>
        <h1>Main Component</h1>
    </div>
    <br>
    <hr>
    <teacherComp  :getUsers="getUserName" />
    <studentComp  />
</template>

<script>
import teacherComp from "./teacher.vue";
import studentComp from "./student.vue";

export default{
    name: "mainComp",
    components: {teacherComp, studentComp},
    methods: {
        getUserName(name){
            alert(name)
        },
        
    }
}
</script>