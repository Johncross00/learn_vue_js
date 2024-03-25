<template>
    <div>
        <h1>Enfant child comp</h1>
        <h2>{{ name }}</h2>
        <h2>{{ userchild.email }}</h2>
        <button v-on:click="passData()" >Call</button>
        <ul>
            <li v-for="item in users" :key="item">
                <!-- {{ item.name }}  -->
                <newUser :data="item"/>


                <!-- &nbsp;{{ item.email }} -->
            </li>
        </ul>
        <h1 v-html="email"></h1>
        <h1 v-html="id"></h1>
        <hr>
        <!-- <newUser :data="users"/> -->
        
    </div>
</template>

<script>
import newUser from "./new-user.vue"
export default{
    name: "childComp",
    props: {
        name: String,
        userchild: Object,
        passData: Function
    },
    data(){
        return {
        //     users: [{
        //         name: "Michel",
        //         email: "michel@gmail.com",
        //     },
        //     {
        //         name: "John",
        //         email: "john@gmail.com",
        //     },
        //     {
        //         name: "Fred",
        //         email: "fred@gmail.com",
        //     }
        // ]
        names: "Peter",
        email: " <h1>peter@gmail.com</h1> ",
        id: "<div>1010101015</div>"
        }
    },
    components: {
        newUser
    }
}
</script>
<style scoped>
li{
    color: rgb(30, 233, 16);
}
</style>