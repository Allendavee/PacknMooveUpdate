<template>
   <Navbar />
    
</template>

<script>
import Navbar from "../components/Navbar.vue"
export default {
    name: 'Services',
    mounted(){
        document.title = 'Services | Packnmoove.com.ng'
    },

    components: {
      Navbar
    },    
}
</script>

<style scoped>

</style>