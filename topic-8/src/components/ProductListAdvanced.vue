// Create a catalog of products, each product having the following properties:
// Name of product
// Price of the product
// Type of product (whether it is digital or physical)
// Whether the product has one or more of the following characteristics:
// Fragile
// Discount
// Limited edition

// Using the techniques in this section, create a ProductListAdvanced and Product component. 
// The former component should render a list of Product components.

<template>
    <div>
        <Product v-for="p in products" v-bind:key="p.id" v-bind:product="p"></Product>
    </div>
</template>
<script>
import Product from "./Product"
export default {
    components:{
        Product
    },
    data:function(){
        return {
            products:[
                {
                    id:'001',
                    name:'poster',
                    price:15,
                    type:'physical',
                    characteristics:['limited edition', 'discount']
                },
                {
                    id:'002',
                    name:'album',
                    price:40,
                    type:'digital',
                    characteristics:['limited edition']
                },
                {
                    id:'003',
                    name:'lightstick',
                    price:20,
                    type:'physical',
                    characteristics:['fragile']
                }
            ]
        }
    }
}
</script>
<style scoped>

</style>