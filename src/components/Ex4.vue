<script>
    export default { 
        data() {
            return {
                // Add code here
                currentColor: "redBox",
                id: "demo1"

            }
        },
        methods: { 
   			// Add code here
            changeColor(){
                this.currentColor = this.currentColor === "redBox" ? "blueBox" : "redBox";
            }
            

		}
    }
</script>

<template>
    
    <!-- Modify code here -->
    <div class="container">
        <div v-bind:id="id" :class="[currentColor, 'm-2']">
            div ID : {{id}} 
        </div>
        <button type="button" @click="changeColor">Change Color</button>
    </div>

</template>

<style scoped>
    .redBox {
        background-color: red;
    }
    .blueBox {
        background-color: blue;
        color: white;
    }
    #demo1 {
        color: white;
    }
</style>
