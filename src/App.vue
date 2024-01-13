<template>
  <v-app >
    
    <v-main >
      
      <v-img
        src="/images/Mountains.jpg" 
        cover
        lazy-src="/images/Mountains.jpg"
        max-height="959"
        
      >
      
        <!--<Navigation/>-->
      <v-container fluid>
        <v-row>
        <v-col cols="2" md="2" class="menuBar">
          <Navigation/>
        </v-col >
        <v-col cols="12" md="3" class="content"   >
            <ContentsTemplate/>
    
        </v-col>
      </v-row>
      </v-container>
        
          <!--<v-sheet  :elevation="elevation" height="1300" width="1300" rounded color="rgba(0, 0, 0, 0.4)"  class="mx-auto" ></v-sheet>-->

         
        
        
      </v-img>
      
    </v-main>
  </v-app>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Navigation from './components/NavigationVue.vue';
import ContentsTemplate from './components/ContentsTemplate.vue';



export default {
  name: 'App',

  components: {
    //HelloWorld,
    Navigation,
    ContentsTemplate

    
  },

  data: () => ({
    //
  }),
}
</script>

<style>
.menuBar {
  position: fixed;
  height: 100vh;
  /* Optionally, add any other styling you need for the fixed navigation */
}
.content{
  position: absolute;
  top: -0%;
  left: 16%;
  
}

.content p{
  color: white;
}

.BodyDesign::-webkit-scrollbar {
  display: none;
}
</style>
