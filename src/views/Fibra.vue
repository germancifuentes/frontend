<template>
  <main>
    <Barra />
    <v-container fluid grid-list-lg text-lg-left>
      <v-card outline>
        <v-card-title>
          Fibra Optica
        </v-card-title>
        <p class=" text-center pa-2">
            La fibra hasta el hogar (FTTH), también llamada fibra hasta las instalaciones (FTTP), es la instalación y el uso de fibra 
            óptica desde un punto central directamente a edificios individuales como residencias, edificios de apartamentos y empresas para proporcionar acceso 
            a internet de alta velocidad.
          </p>
        <v-divider />
        <v-card-text>
            
          <v-row>
            <v-col cols="12" ms="6" sm="4" v-for="(row, index) in productos" :key="index">
            
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
  name: "Fibra",

  components: {
    Barra,
    Producto,
  },
  data: () => ({
    productos: [
      { id: 1 },
      { id: 2 },
      { id: 3 },
      { id: 4 },
      { id: 5 },
      { id: 6 },
      { id: 7 },
    ],
  }),
};
</script>
