<template>
  <main>
    <Barra />
    <v-container fluid grid-list-lg text-lg-left>
      <v-card outline>
        <v-card-title>
          Cobre mediante cableado UTP 
        </v-card-title>
        <p class=" text-center pa-2">
            UTP (Unshielded Twisted Pair – Par trenzado no apantallado): Es un cable sin apantallamiento. Esto lo sigue haciendo 
            bueno para utilizar en casa, por ejemplo, para conectar tu ordenador, NAS o cualquier otro dispositivo al router. Pero es el menos indicado 
            para ser utilizado en instalaciones que van por dentro de la pared y requieren de cables especialmente largos.
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
  name: "Cobre",

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
      
    ],
  }),
};
</script>