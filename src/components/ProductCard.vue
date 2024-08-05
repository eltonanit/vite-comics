<script>
export default {
    props:{
        pathImage: String,
        title: String 
    }
    
}
</script>

<template lang="">
    <div class="col-12 col-md-3 p-0">
        <div class="p-0 m-0 product-card">
            <img :src="pathImage" :alt="title" >
            <h6 class="text-center text-bold">{{title}} </h6>
            </div>
    </div>
        
</template>

<style lang="scss" scoped>

.product-card{
    border:1px solid lightcoral;
}
    
</style>