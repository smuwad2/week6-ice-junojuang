<script>
    export default { 
        // Add Code Here
        // challenge: use array
        data(){
            return{
        fruits: ["apple", "orange", "banana"]
            }
        }  
    }
</script>

<template>
    <div id="app">
        <h3>Using Array</h3>
        <span v-for="fruit in fruits" :key="fruit">
            {{ fruit }}<input type="radio" name="fruit">
        </span>
    
    </div>
</template>

<style scoped>
</style>
