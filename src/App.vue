<template>
  <v-app>
    <nav-bar/>
    <v-main>
      <router-view/>
    </v-main>
    <Footer/>
  </v-app>
</template>

<script>
import NavBar from '@/components/NavBar.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',

  data: () => ({
    //
  }),
  components:{
    'nav-bar': NavBar,  
    Footer 
  }
}
</script>
