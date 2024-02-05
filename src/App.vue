<script >
import Navbar from '../src/components/Navbar.vue'
import leftnavbar from '../src/components/leftnavbar.vue'
import carosello from '../src/components/carosello.vue'
import esplora from '../src/components/explorer.vue'
export default{
  components:{ Navbar,leftnavbar, carosello,esplora}
  }

</script>

<template>


<Navbar/>
<leftnavbar/>
<carosello/>
<esplora/>
</template>

<style scoped lang="scss" >

a{
  text-decoration: none;
}

</style>
