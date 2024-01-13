
import { VNavigationDrawer } from 'vuetify/lib/components/index.mjs';
<template>
      <v-layout>
        <v-navigation-drawer
    
        expand-on-hover
          rail
          color="rgba(0, 0, 0, 0.2)"
          width="300"
          app
          
        >
          <v-list >
            <v-list-item
              prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
              title="Ibrahim George"
              subtitle="ibrahimgeorge1@gmail.com"
            ></v-list-item>
          </v-list>
  
          <v-divider></v-divider>
  
          <v-list density="compact" nav>
            <v-list-item prepend-icon="mdi-account-details" title="About Me" value="aboutme"></v-list-item>
            <v-list-item prepend-icon="mdi-note" title="Articles" value="articles"></v-list-item>
            <v-list-item prepend-icon="mdi-file-code" title="Solutions" value="Solutions"></v-list-item>
          </v-list>
        </v-navigation-drawer>
        <v-main style="height: 220px; ;"></v-main>
      </v-layout>
    
  </template>



