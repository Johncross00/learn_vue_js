<template>
    <div>
        <h1>Watcher</h1>
        <h2>{{ counter }}</h2>
        <button v-on:click="counter = counter+1">+</button>
        <button v-on:click="counter = counter-1">-</button>
        
    </div>
</template>

<script>


export default{
    name: "watcherComp",
    data() {
        return {
            counter: 0
        }
    },
    watch: {
        counter(num, dingo) {
            if(num > 5 && num > dingo){
                alert("Max");
                this.counter = 0
            }
        }
    }
    
}
</script>