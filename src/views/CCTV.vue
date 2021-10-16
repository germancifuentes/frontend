<template>
  <main>
    <Barra />
    <v-container fluid grid-list-lg text-lg-left>
      <v-card outline>
        <v-card-title>
          Circuito Cerrado de televisión
        </v-card-title>
        <p class=" text-center pa-2">
            Un CCTV o circuito cerrado de televisión es una instalación de equipos conectados que generan un circuito de imágenes que solo 
            puede ser visto por un grupo determinado de personas, estas se personalizan para adaptarse a las necesidades de cada cliente bien sean orientadas a la 
            seguridad, vigilancia o mejora de servicio.
        </p>
        <v-divider />
        <v-card-text>
            
          <v-row>
            <v-col cols="12" ms="6" sm="4" >
              <producto></producto>
            </v-col>
            
          </v-row>
        </v-card-text>
      </v-card>
    </v-container>
  </main>
</template>

<script>
import Barra from "../components/Barra.vue";
import Producto from "../components/Producto.vue";

export default {
  name: "CCTV",

  components: {
    Barra,
    Producto,
  },
  data: () => ({
    productos: [
      { id: 1 },
      { id: 2 },
      
    ],
  }),
};
</script>