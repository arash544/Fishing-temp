<template>
  <div class="wrapper">
      <Textbanner head="INTRODUCING FISHTRIPR MANAGER" title="Powerful tools for modern fishing business" txt="Fishtripr Manager is the smart way to manage your fishing business online. Custom website, Flexible payments, booking button, chat system - all together for the first time." link="Learn more >"/>
      <Imagebanner/>
  </div>
</template>

<script>
import Textbanner from './Textbanner'
import Imagebanner from './Imagebanner'
export default {
name:'Banner',
components:{
    Textbanner,
    Imagebanner
}
}
</script>

<style lang="scss" scoped>


.wrapper{
   width: 100%; 
   
}
</style>