<template>
    <div>
        <h4>{{product.name}}</h4>
        <ul>
            <li>Price: {{product.price}}</li>
            <li>Type: {{product.type}}</li>
            <li>Characteristics: {{product.characteristics}}</li>
        </ul>
    </div>
</template>
<script>
export default {
    props:['product']
}
</script>
<style scoped>

</style>