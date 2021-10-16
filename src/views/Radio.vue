<template>
  <main>
    <Barra />
    <v-container fluid grid-list-lg text-lg-left>
      <v-card outline>
        <v-card-title>
          Radio Enlace 
        </v-card-title>
        <p class=" text-center pa-2">
            El Radio Enlace o radioenlace punto a punto, es un sistema de conexiones entre dos o más terminales "antenas" 
            que utilizan ondas electromagnéticas para transmitir datos. Una antena se encargará de enviar la información y la otra se encargará 
            de recibirlos para así facilitar la información hasta en los lugares que sea más difícil por el lugar geográfico o los costes que supondría.
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
  name: "Radio",

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