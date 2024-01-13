<template>
  <v-app >
    
    <v-main >
      <!--Photo by <a href="https://unsplash.com/@danotis?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Dan Otis</a> on <a href="https://unsplash.com/photos/aerial-view-of-pine-trees-in-mist-OYFHT4X5isg?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>-->
      <!--Photo by <a href="https://unsplash.com/@toastyraw?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Pascal M.</a> on <a href="https://unsplash.com/photos/brown-trees-with-sun-rays-rckx2mE9rOw?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
  -->
      <v-img
        src="/images/forestlarge.jpg" 
        cover
        lazy-src="/images/forestsmall.jpg"
        height="959"
        
      >
      
        <!--<Navigation/>-->
      <v-container fluid>
        <v-row>
        <v-col cols="2" md="2" class="menuBar">
          <Navigation @Page="HandlePage"/>
        </v-col >


        <v-col cols="12" md="3" class="content" v-if="PageToDisplay === ''">
            <!--<ContentsTemplate/>-->
            <AboutMe @Page="HandlePage"/>
        </v-col>
       
        <v-col cols="12" md="3" class="content" v-if="PageToDisplay === 'aboutme'  ">
            <AboutMe @Page="HandlePage"/>
        </v-col>
     
      <v-col cols="12" md="3" class="content" v-if="PageToDisplay === 'articles'  ">
            <ArticlesSection/>
        </v-col>
     
      <v-col cols="12" md="3" class="content" v-if="PageToDisplay === 'solutions'  ">
            <SolutionSection/>
        </v-col>
      

      </v-row>

      <v-sheet class="pa-2 ma-2 Footer" width="1298" color="rgba(0, 0, 0, 0.0)">
      <v-row justify="center" align="center">
        <v-col v-for="item in iconList" :key="item.id" cols="auto">
          <a :href="item.link" target="_blank" v-if="item.type === 'link'" style="color: white;">
            <v-icon size="35" :style="{ color: item.iconColor }">{{ item.icon }}</v-icon>
            {{ item.text }}
          </a>
          <a :href="`mailto:${item.link}`"  v-else-if="item.type === 'mailto'" style="color: white;">
            <v-icon size="35" :style="{ color: item.iconColor }">{{ item.icon }}</v-icon>
            {{ item.text }}
          </a>
        </v-col>
      </v-row>
    </v-sheet>
      </v-container>
        
          <!--<v-sheet  :elevation="elevation" height="1300" width="1300" rounded color="rgba(0, 0, 0, 0.4)"  class="mx-auto" ></v-sheet>-->

         
        
          
      </v-img>
      
      
    </v-main>
  </v-app>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Navigation from './components/NavigationVue.vue';
//import ContentsTemplate from './components/ContentsTemplate.vue';
import AboutMe from './components/Contents/AboutMe.vue'
import SolutionSection from './components/Contents/SolutionsSection.vue'
import ArticlesSection from './components/Contents/ArticlesSection.vue';



export default {
  name: 'App',

  components: {
    //HelloWorld,
    Navigation,
    //ContentsTemplate,
    AboutMe,
    SolutionSection,
    ArticlesSection,


    
  },

  data(){
    return{
      PageToDisplay: '',
      iconList: [
        { id: 1,  icon: 'mdi-linkedin',link: 'https://www.linkedin.com/in/ibrahim-g-393955119/', text: '',type: 'link',iconColor: 'white' },
        { id: 2,  icon: "mdi-github",link: 'https://github.com/IbyG', text: '',type: 'link' },
        { id: 3,  icon: "mdi mdi-email",link: 'ibrahimgeorge1@gmail.com', text: '',type: 'mailto' },
      ],
    }
  },
    methods: {
      HandlePage(pageName){
        this.PageToDisplay = pageName;
      }
    }
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

.Footer{
  position: absolute;
  top: 94%;
  Left: 16.3%;
}
</style>
