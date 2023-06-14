<!-- script is where the JS code goes -->
<script setup> // <-- 'setup' is added here to enable the new syntax for Vue 3, for using the composition API -->

// ref is a function from the 'vue' package that is imported from vue
// it will be used to create a reactive reference 
import { ref } from 'vue'

// props are a way to pass data from a parent component to a child component
// it is a mechanism for communication between components in a Vue application
// it will be used to pass the 'msg' prop from the parent component to this child component 
defineProps({
    msg: String, // 'msg' is the name of the prop, and 'String' is the type of the prop to be passed from the parent component to this child component
})

</script> <!-- end of JS code -->

<!-- Beginning of the template. where the HTML goes -->
<template>

    <!-- We insert the msg that we previously defined into the HTML -->
    <h1>{{ msg }}</h1>

    <div class="jumbotron">
        
    </div>

</template>

<!-- 'scope' makes my CSS exclusive to this component -->
<style scoped>
    .jumbotron
    {
        width: 1200px;
        height: 600px;
        background-color: #f0f0f0;
        text-align: center;
    }
    
</style>
