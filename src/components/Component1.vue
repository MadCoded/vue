<template>
<div>
    <span style="color:chartreuse"> Static </span>
    <br>
    <span> {{ testData }} </span>

</div>
</template>


<script>
    export default {
        name: "Component1",
        data() {
            return {
                testData: "Component1"
            }
        }


    }

</script>


<style scoped>
    span {
        color: white;
        font-weight: bold;
    }
    div{
        height: 500px;
        width: 300px;
        background-color: #35495e;
          float: left;
          border-radius: 5px;
          margin-left: 5px;
    }
</style>