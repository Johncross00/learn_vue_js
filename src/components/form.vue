<template>
    <div>
        <h1>Formulaire</h1>
    </div>
    <form action="">
        <label for="">Username</label>&nbsp;
        <input type="text" name="" id="" v-model="form.username"> <br> <br>

        <label for="">Password</label>&nbsp;
        <input type="password" name="" id="" v-model="form.password"> <br> <br>

        <button v-on:click="login">Sign Up</button>

        <p>{{ form }}</p>

        <br><br>
        <label for="">Hobbies {{ Hobbies }}</label> <br>
        <label for="">Enduro</label>
        <input type="checkbox" name="" id="" value="Enduro" v-model="Hobbies"><br>
        <label for="">Cross</label>
        <input type="checkbox" name="" id="" value="Cross" v-model="Hobbies"><br>
        <label for="">Trial</label>
        <input type="checkbox" name="" id="" value="Trial" v-model="Hobbies"><br>
        <br><br><br>

        <label for="">Gender {{ Gender }}</label> <br>
        <label for="">Male</label>
        <input type="radio" name="gender" id="" value="Male" v-model="Gender"><br>
        <label for="">Female</label>
        <input type="radio" name="gender" id="" value="Female" v-model="Gender"><br>
    </form> 

    
    <ul>
        <li v-for="item in fun" v-bind:key="item">
            {{ item }} Not subbmitted
        </li>
    </ul>
</template>

<script>


export default{
    name: "formComp",
    data() {
        return {
            form: {
                username: "",
                password: "",
                Hobbies: [],
                Gender: '',
            },
            fun: []
        };
    },
    methods:{
        login() {
            for (const item in this.form) {
                if(this.form[item] === '' || this.form[item].length === 0) {
                    this.fun.push(item);
                }
            }
            console.table("Login data", this.form, this.fun)
        }
    }
};
</script>