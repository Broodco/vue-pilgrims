<template>
    <div>
        <ul>
            <li v-for="pilgrim in pilgrims" :key="pilgrim">
                <Item :source="pilgrim"></Item>
            </li>
        </ul>
    </div>
</template>

<script>
import Item from './Item.vue'

export default {
    name : "List",
    components: {
        Item
    },
    props:{
        pilgrims: Array
    }
}
</script>

<style scoped>
div{
    padding: 0.2rem;
}
ul{
    padding: 0;
}
li{
    list-style: none;
}
</style>
