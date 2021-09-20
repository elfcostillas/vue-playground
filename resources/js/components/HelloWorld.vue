<template>
    from template <br>
    <span> {{ greeting }} </span>
    <button @click=changeTitle>123</button>

    <div v-for="fruit in fruits" > <span> {{fruit}} </span> </div>

        <div v-for="name in names.employee" > <span> {{name.idno}} - {{name.name}} - {{name.department}} </span> </div>
    
</template>
<script>
//import { ref } from 'vue'
export default {
    // setup:() => ({
    //     greeting: 'Hello World from Vue 3!',
    //     changeTitle(){
    //         // some code
    //         //this.title
    //         console.log(this.greeting)
    //     },
       


      
    // }),

    setup () {
        let greeting = 'welcome to vue js'
        let fruits = ['apple','mango','grapes','coconut','straberry']
        let names = {
           "employee" : [
                { idno : 1, name : "edgar" , department : "IT"},
                { idno : 2, name : "alan" , department : "IT"},
                { idno : 3, name : "mia" , department : "IT"},
                { idno : 4, name : "Lexi" , department : "IT"},
           ]
        }

        return {
            greeting,
            fruits,
            names
        }
    }
    

}


</script>