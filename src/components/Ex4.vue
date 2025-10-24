
<script>
    export default { 
        data() {
            return {
                // Add code here
                    id: "demo1",       // bind to the div id
                    isBlue: true
            }
        },
        methods: { 
   			// Add code here
            toggleColor() {
            this.isBlue = !this.isBlue;
        
		}
    }
    }
</script>

<template>
    
    <!-- Modify code here -->
    <div class="container">
        <div :id="id" class="m-2" :class="{ 'blueBox': isBlue, 'redBox': !isBlue }">
            div ID : {{id}} 
        </div>
        
        <button type="button" :class="{'btn btn-primary':isBlue, 'btn btn-danger': !isBlue}"
        v-on:click="toggleColor">Change Color</button>
    </div>

</template>

<style scoped>
    .redBox {
        background-color: red;
    }
    .blueBox {
        background-color: blue;
    }
    #demo1 {
        color: white;
    }
</style>
