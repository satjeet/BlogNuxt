<template>
  <div>
    <TheHeader @sidenavToggle="displaySidenav=!displaySidenav"/>
    <TheSidenav :show="displaySidenav" @close="displaySidenav=false"/>

    <nuxt />
  </div>
</template>

<script>
  import TheHeader from '@/components/Navegation/TheHeader'
  import TheSidenav from '@/components/Navegation/TheSidenav'


export default{
  components:{
    TheHeader,
    TheSidenav,
  },
  data(){
    return{
      displaySidenav:false
    }
  },
}
</script>
<style>
html{
  font-family:'Open Sans', sans-serif;
}
body{
  margin:0;
}
</style>
