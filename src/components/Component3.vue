<template>
<span>
    {{com3Data}}
</span>
</template>


<script>
export default{
    name: "Component3",
    data(){
        return{
            com3Data : "Compoenent3 Nested"
        }
    }
}
</script>



<style scoped>
    span{
        border : 3px solid black;
        border-radius: 10px 5px;
        padding:  10px;
        margin-top: 50px
    }
</style>