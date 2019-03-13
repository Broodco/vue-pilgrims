<template>
    <div class="box">
        <div class="image">
            <img :src="source.img" alt="avatar">
        </div>
        <div class="texts">
            <div class="nom">
                {{ source.name }}
            </div>
            <div class="desc">
                {{ source.desc }}
            </div>
        </div>
    </div>
</template> 

<script>
export default {
    name : "Item",
    props:{
        source : Object
    }
}
</script>

<style scoped>
.box{
    height : 7rem;
    padding: 0.5rem;
    border : 1px solid black;
}
.texts{
    height:7rem;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
}
.image{
    height : 7rem;
    float:left;
}
img{
    height:100%;
}
</style>
