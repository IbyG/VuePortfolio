
import { VNavigationDrawer } from 'vuetify/lib/components/index.mjs';
<template>
      <v-layout>
        <v-navigation-drawer
    
        expand-on-hover
          rail
          color="rgba(0, 0, 0, 0.4)"
          width="300"
          app
          
        >
          <v-list >
            <v-list-item
                prepend-avatar="./images/headshot2024.png"
                title="Ibrahim George"
                style="color: white;"
            >
                <template v-slot:subtitle>
                <a :href="'mailto:' + 'ibrahimgeorge1@gmail.com'" style="color: white;">ibrahimgeorge1@gmail.com</a>
                </template>
            </v-list-item>
          </v-list>
  
          <v-divider></v-divider>
  
          <v-list density="compact"  nav>
            <v-list-item prepend-icon="mdi-account-details" title="About Me" value="aboutme" @click="shareWithApp('aboutme')" style="color: white;"></v-list-item>
            <v-list-item prepend-icon="mdi-note" title="Articles" value="articles" @click="shareWithApp('articles')" style="color: white;"></v-list-item>
            <v-list-item prepend-icon="mdi-file-code" title="Solutions" value="olutions" @click="shareWithApp('solutions')" style="color: white;"></v-list-item>
          </v-list>
        </v-navigation-drawer>
        <v-main style="height: 220px; ;"></v-main>
      </v-layout>
    
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
