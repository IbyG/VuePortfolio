<template>
    <v-sheet   :elevation="elevation" height="900"  width="1300" color="rgba(0, 0, 0, 0.7)" class="scrollable-sheet"  >
                <p class="text-center text-h1 ">This is the About Me Page</p>
                <p>About Me Section....
              
                </p>
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