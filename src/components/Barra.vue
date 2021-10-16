<template>
  <v-card class="overflow-hidden">
    <v-app-bar
      
      color="#6A76AB"
      dark
      shrink-on-scroll
      prominent
      src="https://i.ibb.co/ftmzkVt/Ciudad-Conectada.jpg"
      fade-img-on-scroll
      scroll-target="#scrolling-techniques-3"
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(100,115,201,.7), rgba(25,32,72,.7)"
        ></v-img>
      </template>

      

      <h3>Nuestros Servicios</h3>

      <v-spacer></v-spacer>

      

      <template v-slot:extension>
        <v-tabs align-with-title>
          <v-tab href="/fibra">Fibra Optica</v-tab>
          <v-tab href="/cobre">Cobre Utp</v-tab>
          <v-tab href='/cctv'>CCTV</v-tab>
          <v-tab href="/radio">Radio</v-tab>
          
          <!--<v-tab href="/productos">productos</v-tab>-->
        </v-tabs>
      </template>
    </v-app-bar>
    <v-sheet
      id="scrolling-techniques-3"
      class="overflow-y-auto"
      max-height="600"
    >
      
    </v-sheet>
  </v-card>
</template>
<script>
export default {
    data(){

    },
    
}
</script>