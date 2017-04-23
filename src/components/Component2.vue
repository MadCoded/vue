<template>
    <div>
       <span style="color:violet" class=bold> Dynamic </span>  
        <br>
        <span> {{ testData }} </span>
        <ul>
            <li v-for="user in users">
                {{user.name}} ({{user.username}})
            </li>
        </ul>
        <br><br>
        <component3></component3>
    </div>
</template>

<script>
    import Component3 from './Component3.vue';

    export default {
        name: "Component2",
        data() {
            return {
                testData: "Component2",
                users : []
            }
        },
        components: {
            Component3
        },
        created: function(){
            this.$http.get('https://jsonplaceholder.typicode.com/users')
                .then(function(response){
                    //console.log(response.body);
                    this.users =  response.body;
                });
        }

    }

</script>



<style scoped>
    span {
        color: white;
    }
    
    div {
        width: 300px;
        height: 500px;
        background-color: #41b883;
        float: left;
        display: inline;
        border-radius: 5px;
        margin-left: 5px;
    }
    ul{
        text-align: left;
    }
    .bold{
        font-weight: bolder;
    }
</style>