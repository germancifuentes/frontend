<template>
  <main>
    <Barra />
    <v-container fluid grid-list-lg text-lg-left>
      <v-card outline>
        <v-card-title>
          PLANES 
        </v-card-title>
        <v-divider />
        <v-card-text>
            <v-row>
                <v-col cols="10" md="10" sm="12">
                    <v-text-field
                    label="Buscar producto"
                    outlined
                    dense>
                    </v-text-field>
                </v-col>
                <v-col cols="2" md="2" sm="12">
                </v-col>
            </v-row>
          <v-row>
            <v-col cols="12" ms="6" sm="4">
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
  name: "Productos",

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