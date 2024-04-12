<template>
    <div class="card">
        <h1>Slots</h1>
        <slot name="header"></slot>        
        <slot name="main"></slot>        
        <slot name="footer"></slot>        
    </div>
</template>

<script>


export default{
    name: "slotComp",
    props: {
        data: String
    }
}
</script>
<style>
.card{
    background-color: aqua;
    border: 1px solid;
    width: 250px;

}
</style>