<template>
    <div>
        <h1>Product List</h1>
        <div>
            <input type="text" v-model="newProduct" placeholder="Enter New Product"/>
            <button v-on:click="addNewProduct">Add New Product</button>
        </div>
        <p v-for="p in products" v-bind:key='p'>{{p}}<button v-on:click="deleteProduct(p)">Delete Product</button></p>
    </div>
</template>
<script>
export default {
    data:function(){
        return{
            'products':['handbags', 'vacuum cleaner', 'gold watch'],
            // 'newProduct':''
        }
    },
    methods:{
        addNewProduct:function(){
            this.products.push(this.newProduct)
            this.newProduct=""
        },
        deleteProduct:function(product){
            let indexOfProduct = this.products.indexOf(product);
            this.products.splice(indexOfProduct,1)
        }
    }
}
</script>
<style scoped>

</style>