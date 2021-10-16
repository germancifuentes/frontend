<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <h1>INTERNET SERVICE PROVIDER</h1>
      </div>

      <v-spacer></v-spacer>
      <v-row align="baseline" justify="end">
        <v-btn text href="/">
          Inicio
        </v-btn>
        <v-btn text href="/fibra">
          Servicios
        </v-btn>
        <v-btn text>
          Contactanos
        </v-btn>
        <v-btn text href="/Login">
          Login
          <v-avatar color="primary">
            <v-icon dark>
              mdi-account-circle
            </v-icon>
          </v-avatar>
        </v-btn>
      </v-row>
    </v-app-bar>

    <v-main class="blue-grey lighten-5">
      <router-view />
    </v-main>
    <v-footer
    dark
    padless
  >
    <v-card
      class="flex"
      flat
      tile
    >
      <v-card-title class="primary">
        <strong class="subheading">Conéctate con nosotros en las redes sociales!</strong>

        <v-spacer></v-spacer>

        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4"
          dark
          icon
        >
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>
      </v-card-title>

      <v-card-text class="py-2 white--text text-center">
        {{ new Date().getFullYear() }} — <strong>
Copyright - Misiontic2022 - UTP</strong>
      </v-card-text>
    </v-card>
  </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    //
  }),
};
</script>
<script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>
<style>
.text {
  color: darkblue;
}
.imgn:hover {
  cursor: pointer;
  filter: grayscale(90%);
  
}

</style>
