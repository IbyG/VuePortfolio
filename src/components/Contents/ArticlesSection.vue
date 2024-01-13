<template>
    <v-sheet :elevation="elevation" height="900"  width="1300" color="rgba(0, 0, 0, 0.4)" class="scrollable-sheet"  >
        <p class="text-center text-h1 ">Articles</p>
        <v-container class="transparent-container" fluid>
            <v-row no-gutters >
            <v-col >
                <v-sheet class="pa-2 ma-2" color="transparent">
                    <v-row justify="center" >
                        <v-img src="/images/server.jpeg" max-width="400" max-height="400" />
                    </v-row>
                    <br>
                    <p class="text-h5 text-left">SCALING HEIGHTS: A YEAR-LONG HOMELAB EXPEDITION AND WHAT LIES AHEAD</p> <br>
                    <p>Embark on a captivating journey through a year-long exploration of building and scaling a homelab server.</p>
                    <!--Button-->
                    <v-row class="pa-2 ma-2" justify="center" align="center"  >
                    <v-col cols="auto">
                        <v-btn rounded href="https://www.linkedin.com/posts/ibrahim-g-393955119_homelabadventures-selfhosting-techjourney-activity-7147753538549350400-PpCJ?utm_source=share&utm_medium=member_desktop" target="_blank">Learn More</v-btn>
                    </v-col>
                    </v-row>
                </v-sheet>
            </v-col>
            <v-col >
                <v-sheet class="pa-2 ma-2" color="transparent">
                    <v-row justify="center" >
                        <v-img src="/images/fundoimage.png" max-width="400" max-height="400" />
                    </v-row>
                    <br>
                    <p class="text-h5 text-left">FUNDO ETL</p> <br>
                    <p>In my recent exploration of fitness data processing, I've shared insights on how we automated the extraction and analysis of data from the Fundo app using our Fundo ETL solution.</p>
                    <!--Button-->
                    <v-row class="pa-2 ma-2" justify="center" align="center"  >
                    <v-col cols="auto">
                        <v-btn rounded href="https://www.linkedin.com/posts/ibrahim-g-393955119_dataautomation-etl-bashscripting-activity-7145601197909917696-5joT?utm_source=share&utm_medium=member_desktop" target="_blank">Learn More</v-btn>
                    </v-col>
                    </v-row>
                </v-sheet>
            </v-col>

            <v-responsive width="100%"></v-responsive>

            <v-col >
                <v-sheet class="pa-2 ma-2" color="transparent">
                    <v-row justify="center" >
                        <v-img src="/images/superset.jpeg" max-width="400" max-height="400" />
                    </v-row>
                    <br>
                    <p class="text-h5 text-left">FROM METRICS TO INSIGHTS: TRANSFORMATIVE EXPERIENCE WITH SUPERSET</p> <br>
                    <p>Dive deeper into the transformative world of Superset a self-hosted analytics BI platform</p>
                    <!--Button-->
                    <v-row class="pa-2 ma-2" justify="center" align="center"  >
                    <v-col cols="auto">
                        <v-btn rounded href="https://www.linkedin.com/posts/ibrahim-g-393955119_supersetjourney-datavisualization-homelabadventure-activity-7148592666304217088-WNUi?utm_source=share&utm_medium=member_desktop" target="_blank">Learn More</v-btn>
                    </v-col>
                    </v-row>
                </v-sheet>
            </v-col>

            <v-col >
                <v-sheet class="pa-2 ma-2" color="transparent">
                    <v-row justify="center" >
                        <v-img src="/images/shopify-subscriptions.png" max-width="400" max-height="400" />
                    </v-row>
                    <br>
                    <p class="text-h5 text-left">AUTOMATING RECURRING PAYMENTS: A DEEP DIVE INTO SHOPIFY-ZOHO SUBSCRIPTIONS INTEGRATION</p> <br>
                    <p>Maximise the power of your Shopify store by seamlessly integrating with Zoho Subscriptions, ensuring effortless order management and automated recurring payments to propel your e-commerce success.</p>
                    <!--Button-->
                    <v-row class="pa-2 ma-2" justify="center" align="center"  >
                    <v-col cols="auto">
                        <v-btn rounded >Learn More</v-btn>
                    </v-col>
                    </v-row>
                </v-sheet>
            </v-col>

            <v-responsive width="100%"></v-responsive>
           
            </v-row>
        </v-container>

        </v-sheet>
  </template>
  
  <script>
  export default {
  
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