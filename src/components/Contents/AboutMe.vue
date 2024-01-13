<template>
    <v-sheet   :elevation="elevation" height="900"  width="1300" color="rgba(0, 0, 0, 0.4)" class="scrollable-sheet"  >
        
                <p class="text-center text-h1 ">About Me</p>
                <p class="text-center">I have over half a decade of experience working in solution architecture, consulting, account management and data analyses. I am currently fulfilling the role of a solution architect and account manager at Customer Consulting Group. This role involves me working with an incredible cross-functional team which assists the CCG client base with solution designs to assist in optimising and automating their current business process flow.
                </p>
                <br>
                <p class="text-center">In my career I am deeply passionate about implementing a simple but effective system user experience that helps the client achieve their desired outcomes. If you catch me outside of work however, I have a green thumb and love to talk about plants and gardening – and I dabble a bit into woodworking.
                </p>           
                
                <br><br>
                <p class="text-h5 text-center">Competencies</p>
                <br>
				
                <v-sheet class="pa-2 ma-2" width="1298"  color="rgba(0, 0, 0, 0.0)">
                    <v-row justify="center" align="center"  >
                        <a><img class="ma-1" src="/images/python-colored.svg" width="36" height="36" alt="Python" /></a>
                        <a><img class="ma-1" src="images/js.png" width="36" height="36" alt="Javascript" /></a>
                        <a><img class="ma-1" src="images/git.png" width="36" height="36" alt="Git" /></a>
                        <a><img class="ma-1" src="images/c-.png" width="36" height="36" alt="C++" /></a>
                        <a><img class="ma-1" src="images/visual-basic.png" width="36" height="36" alt="visual-basic" /></a>
                        <a><img class="ma-1" src="images/java (1).svg" width="36" height="36" alt="Java" /></a>
                        <a><img class="ma-1" src="images/vue-js-icon-2048x1766-btrgkrhi.png" width="36" height="36" alt="vuejs" /></a>
                        <a><img class="ma-1" src="images/Mariadb-seal-browntext.svg.png" width="89" height="36" alt="Mariadb" /></a>
                        <a><img class="ma-1" src="images/mysql.svg" width="36" height="36" alt="mysql" /></a>
                        <a><img class="ma-1" src="images/mongodb-icon-1.svg" width="36" height="36" alt="mongodb" /></a>
                        <a><img class="ma-1" src="images/docker.png" width="36" height="36" alt="docker" /></a>
                        <a><img class="ma-1" src="images/1200px-Icons8_flat_linux.svg.png" width="36" height="36" alt="Linux" /></a>
                        <a><img class="ma-1" src="images/2560px-ZOHO.svg.png" width="100" height="36" alt="Zoho" /></a>
                        <a href="https://public.tableau.com/app/profile/ibrahim.george8707/viz/FundoReports/SportsDashboard#1" target="_blank"><img class="ma-1" src="images/tableau-software.svg" width="36" height="36" alt="Tableau" /></a>
                        <a><img class="ma-1" src="images/superset-icon-logo-D70353ADD5-seeklogo.com.png" width="60" height="36" alt="SuperSet" /></a>
                    </v-row>
                </v-sheet>

                <v-sheet class="pa-2 ma-2" width="1298" height="400" color="rgba(0, 0, 0, 0.0)">
                    <v-row justify="center" align="center"  >
                       <br><br><br>
                        <p class="text-center text-h5" >A BIT ABOUT MY PROJECT HISTORY</p>
                        
                    </v-row>
                </v-sheet>

                <v-row class="pa-2 ma-2" justify="center" align="center"  >
                    <v-col cols="auto">
                        <v-btn rounded @click="shareWithApp('articles')">To Articles</v-btn>
                    </v-col>
                    <!--
                    <v-col cols="auto">
                        <v-btn rounded >To Solutions</v-btn>
                    </v-col>
                    -->
                </v-row>
              </v-sheet>
  </template>
  
  <script>
  export default {
    methods: {
      shareWithApp(value) {
        // Emit an event named 'childMessage' with a message
        this.$emit('Page', value);
        console.log(value)
      }
    }
  }
  </script>
  
  <style>
  .scrollable-sheet {
    max-height: 910px; /* Set a maximum height if needed */
    overflow-y: auto; /* Enable vertical scrolling */
  }
  
  /* Hide the scrollbar for WebKit-based browsers */
  .scrollable-sheet::-webkit-scrollbar {
    display: none;
  }
  </style>