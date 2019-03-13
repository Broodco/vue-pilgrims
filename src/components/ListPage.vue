<template>
    <div>
        <Header title="List of the Pilgrims"></Header>
        <SearchBar></SearchBar>
        <List :pilgrims="pilgrims"></List>
    </div>
</template>

<script>
import Header from './Header.vue'
import List from './List.vue'

export default {
    name : "ListPage",
    components:{
        Header,
        List
    },
    props:{
        pilgrims : Array
    },
    data(){
        return{
            pilgrims: pilgrims
        }
    }
};
</script>

<style scoped>
div{
    border: 2px solid red;
    display: flex;
    flex-direction: column; 
    justify-content: space-around;
}
</style>
