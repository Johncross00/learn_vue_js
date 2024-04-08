<template>
    <div>
        <h1>Computy Property</h1>
        <span>{{ author.books.length > 0 ? "Oui" : "Non" }}</span> &nbsp;
        <span>{{ publishedBook }}</span>
    </div>
</template>

<script>


export default{
    name: "computyProp",
    data() {
        return {
            author: {
                name: "Popo",
                books: [
                    "Vue 1",
                    "Vue 2",
                    "Vue 3"
                ]
            }
        }
    },
    computed: {
        publishedBook(){
            return this.author.books.length > 0 ? "Yes" : "No"
        }
    }
}
</script>