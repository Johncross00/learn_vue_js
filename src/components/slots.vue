<template>
    <div>
        <h1>Slots</h1>
        <slot></slot>        
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