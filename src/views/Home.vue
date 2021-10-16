<template>
  <main>
    <v-carousel height="300" cycle>
      <v-carousel-item
        v-for="(item, i) in items"
        :key="i"
        :src="item.src"
        reverse-transition="fade-transition"
        transition="fade-transition"
      ></v-carousel-item>
      <v-divider />
    </v-carousel>

    <v-container mt-5 grid-list-xl>
      <v-layout justify-center my-2>
        <v-flex xs5>
          <h1 class="text display-2 text-center">QUIENES SOMOS</h1>
          <v-divider class="blue mt-3"/>
        </v-flex>
      </v-layout>
      <v-layout my-2>
        <v-flex>
          <p class=" text-center pa-2">
            Radio Enlace o radioenlace punto a punto, es un sistema de
            conexiones entre dos o más terminales "antenas" que utilizan ondas
            electromagnéticas para transmitir datos. Una antena se encargará de
            enviar la información y la otra se encargará de recibirlos para así
            facilitar la información hasta en los lugares que sea más difícil
            por el lugar geográfico o los costes que supondría.
          </p>
        </v-flex>
      </v-layout>
      <h1 class="text display-1 text-center">NUESTROS SERVICIOS</h1>
      <v-divider class="blue my-2"/>
      <v-row class="my-5">
        <v-col cols="6" sm="4">
          <v-img
            class="imgn"
            height="235"
            src="https://i.ibb.co/pyP6CfL/Internet-Fibra-Optica1.jpg"
            @click="llamarFibra()"
          ></v-img>
        </v-col>

        <v-col cols="6" sm="4">
          <v-img
            class="imgn"
            height="235"
            src="https://i.ibb.co/8P045N0/Radio-Enlace1.jpg"
            @click="llamarRadio()"
          >
            <div class="fill-height bottom-gradient"></div>
          </v-img>
        </v-col>

        <v-col cols="6" sm="4">
          <v-img
            class="imgn"
            height="235"
            src="https://i.ibb.co/12Zx6dc/Internet-Por-Cobre1.png"
            @click="llamarFibra()"
          >
            <div class="fill-height repeating-gradient"></div>
          </v-img>
        </v-col>

        <v-col cols="6" sm="4">
          <v-img
            class="imgn"
            height="235"
            src="https://i.ibb.co/zPRKJm1/CCTV4.jpg"
            @click="llamarFibra()"
          ></v-img>
        </v-col>

      </v-row>
    </v-container>
    <section id="Testimonios" class="mt-5">
        <h1 class="text display-1 text-center">Testimonios de Nuestros Clientes Satisfechos</h1>
         
          <template>
            <v-timeline>
              <v-timeline-item
                 v-for="n in 1"
                :key="n"
                 large
              >
                <template v-slot:icon>
                  <v-avatar>
                   <img src="https://i.ibb.co/SyNspcm/Roberto-Gomez.jpg">
                  </v-avatar>
                </template>
                <template v-slot:opposite>
                  <span>06 Marzo 2020</span>
                </template>
                <v-card class="elevation-2">
                  <v-card-title class="text-h4">
                    Roberto Gomez
                  </v-card-title>
                  <v-card-text>Excelente Servicio, el internet funciona super bien</v-card-text>
               </v-card>
              </v-timeline-item>
            </v-timeline>
          </template>

          <template>
            <v-timeline>
              <v-timeline-item
                 v-for="n in 1"
                :key="n"
                 large
              >
                <template v-slot:icon>
                  <v-avatar>
                   <img src="https://i.ibb.co/2yWj3vr/Abraham-Lincoln.jpg">
                  </v-avatar>
                </template>
                <template v-slot:opposite>
                  <span>19 Octubre 2020</span>
                </template>
                <v-card class="elevation-2">
                  <v-card-title class="text-h4">
                    Abraham Lincoln
                  </v-card-title>
                  <v-card-text>Me instalaron muy rapido y el soporte es buenisimo</v-card-text>
               </v-card>
              </v-timeline-item>
            </v-timeline>
          </template>      
           <template>
            <v-timeline>
              <v-timeline-item
                 v-for="n in 1"
                :key="n"
                 large
              >
                <template v-slot:icon>
                  <v-avatar>
                   <img src="https://i.ibb.co/smJ2F1Z/Al-Bundy.jpg">
                  </v-avatar>
                </template>
                <template v-slot:opposite>
                  <span>30 julio 2021</span>
                </template>
                <v-card class="elevation-2">
                  <v-card-title class="text-h4">
                    Al Bundy
                  </v-card-title>
                  <v-card-text>Buena empresa ningun otro operador llega al sector donde vivo</v-card-text>
               </v-card>
              </v-timeline-item>
            </v-timeline>
          </template>      
      </section>
  </main>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          src: require("../assets/imagenes home/img-1.jpg"),
        },
        {
          src: require("../assets/imagenes home/img-3.jpg"),
        },
        {
          src: require("../assets/imagenes home/img-4.jpg"),
        },
        
      ],
    };
  },
  methods: {
    llamarproducto() {
      this.$router.push("/productos");
    },
    llamarFibra() {
      this.$router.push("/fibra");
    },
    llamarRadio() {
      this.$router.push("/radio");
    },
  },
};
</script>
