<template>
   
    
    <div v-for="mobile of mobiles" :key="mobile.id" >

     
       <SingleMobile :mobile=mobile />

    </div>

</template>
<script>
import SingleMobile from './SingleMobile.vue'

export default {
    name: 'MobileBox',
    props:{
        mobiles: Array
    },
    components:{
        SingleMobile
    }
    
}
</script>
<style scoped>

</style>
