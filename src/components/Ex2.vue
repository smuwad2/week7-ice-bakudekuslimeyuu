<script>
    export default { 
        // Add code in appropriate places
        data() {
            return {
                items: ['keyboard', 'mouse', 'iPhone', 'macbook', 'adapter'] ,
                AddItem: '' , 
            }  
        } ,
        methods: { 
            AddItem(){ 
                    this.items.push(this.newItem);
                }
            }
        } 
</script>

<template>

    <h2>Shopping Cart</h2>
    <!-- TODO: Add Code Here -->
    <ul v-for = "item in items"> 
        <li> {{ item }}  </li> 
        <button @click = "">Delete</button>
    </ul>

    <p>Additem <input v-model="newItem"></p>
    <button @click = "AddItem">Add!</button>
   
</template>
