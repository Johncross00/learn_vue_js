<template>
    <div>
        <h1>Dans le new user Azalaka Pinhou</h1>
        <h2>Dans le new user: email= {{ data.email }}</h2>
        <h2>Dans le new user: nom= {{ data.name }}</h2>
    </div>
</template>

<script>
export default{
    name: "newUser",
    props: {
        data: Object,
    }
}

</script>