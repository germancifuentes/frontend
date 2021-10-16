<template>
  <v-app>
    <v-main>
      <v-container class="fill-height" fluid>
        <v-row align="center" justify="center" dense>
          <v-col cols="12" sm="8" md="4" lg="4">
            <v-card elevation="0">
              <a href='' name="" title="" target="_blank">
                <v-img src="@/assets/imagenes home/logowifi.png" contain height="200"></v-img>
              </a>
              <v-card-text>
                <v-form>
                  <v-text-field label="Ingresa tu correo" name="email" prepend-inner-icon="mdi-email" type="email" class="rounded-0" outlined></v-text-field>
                  <v-text-field label="Ingresar tu contraseña" name="password" prepend-inner-icon="mdi-lock" type="password" suffix="| Olvido su password?" class="rounded-0" outlined></v-text-field>
                  <v-btn class="rounded-0" color="#000000" x-large block dark>Ingresar</v-btn>
                  <v-card-actions class="text--secondary">
                    <v-checkbox color="#000000" label="Recuerdame"></v-checkbox>
                    <v-spacer></v-spacer>
                    <!-- <router-link :to="{ name: 'SignUp' }">Sign Up</router-link> -->
                    ¿No tienes una cuenta? <a href="#" class="pl-2" style="color: #000000">Acceder</a>
                  </v-card-actions>
                </v-form>
              </v-card-text>
              <v-card-actions class="ml-6 mr-6 text-center">
                <p>Al continuar acepta los terminos y condiciones <a href="#" class="pl-2" style="color: #000000">Politica</a> y <a href="#" class="pl-2" style="color: #000000">Terminos de uso</a></p>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'Login'
}
</script>

<style lang="css" scoped>
</style>
