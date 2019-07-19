<template>
  <v-app>
    <v-container grid-list-md>
      <!-- Grid/Colores/Tipografía/Espaciados -->
      <v-layout wrap>
        <v-flex class="primary" xs12>
          <h1>12</h1>
        </v-flex>
        <v-flex class="success" xs6>
          <h1>6</h1>
        </v-flex>
        <v-flex class="error" xs6>
          <h1>6</h1>
        </v-flex>
      </v-layout>

      <v-layout class="mt-5 secondary" justify-center align-center style="height: 300px">
        <v-flex class="info" xs3>
          <h1>centrado</h1>
        </v-flex>
        <v-flex class="pink lighten-1 white--text" xs3>
          <h1>centrado 2</h1>
        </v-flex>
      </v-layout>

      <v-layout>
        <v-flex>
          <h1 class="display-1 text-uppercase">Display 1</h1>
          <h1 class="display-2 primary pa-5 mt-5">Display 2</h1>
          <h1 class="display-3 text-xs-center">Display 3</h1>
          <h1 class="display-4">Display 4</h1>
        </v-flex>
      </v-layout>
      <hr>
      <!-- Botones e Iconos -->
      <v-layout>
        <v-flex>
          <v-btn>Botão</v-btn>

          <v-btn color="primary">Botão</v-btn>

          <v-btn dark color="blue">Botão</v-btn>

          <v-btn color="pink" flat>sem fundo</v-btn>

          <v-btn color="red" large>largo</v-btn>

          <v-btn color="yellow" small>pequeno</v-btn>

          <v-btn :disabled="true">desabled</v-btn>

          <v-btn color="orange" depressed>depressed</v-btn>

          <v-btn large>
            <v-icon>android</v-icon>
          </v-btn>

          <v-btn color="blue">
            <v-icon>restaurant</v-icon>
          </v-btn>

          <v-btn icon flat>
            <v-icon>cloud_queue</v-icon>
          </v-btn>

          <v-btn color="teal" icon fab>
            <v-icon>usb</v-icon>
          </v-btn>

          <v-btn color="pink" icon fab small>
            <v-icon>duo</v-icon>
          </v-btn>

          <v-btn color="orange" icon fab large>
            <v-icon>sentiment_satisfied_alt</v-icon>
          </v-btn>

          <v-btn color="purple">
            Download
            <v-icon class="ml-2">cloud_download</v-icon>
          </v-btn>

          <v-btn color="success">
            sem outline
            <v-icon class="ml-2">forum</v-icon>
          </v-btn>

          <v-btn color="success" outline>
            com outline
            <v-icon class="ml-2">forum</v-icon>
          </v-btn>

          <v-btn color="error" block>Block</v-btn>

          <div class="text-xs-center">
            <v-btn round color="primary" dark>Botão redondo</v-btn>
          </div>
        </v-flex>
      </v-layout>
      <hr>
      <!-- Navbar Vertical -->
      <v-toolbar dark app class="black">
        <v-toolbar-side-icon @click="drawer = !drawer"></v-toolbar-side-icon>
        <v-toolbar-title>Menu sidebar</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn class="success">Ingresso</v-btn>
        <v-btn class="error">Sair</v-btn>
      </v-toolbar>

      <v-navigation-drawer app v-model="drawer" temporary>
        <v-layout mt-4 column align-center>
          <v-flex>
            <v-avatar>
              <img src="https://media.licdn.com/dms/image/C4D03AQG7-e_d-QJzhQ/profile-displayphoto-shrink_200_200/0?e=1568851200&v=beta&t=_PKUJFV5XfkxwQ6PZC5w9Wz1vJvUyreYTdtPMbM1KX0" alt="">
            </v-avatar>
          </v-flex>
          <v-flex>
            <p class="mt-3 headline">Arthur dos Santos Almeida</p>
          </v-flex>
        </v-layout>
      </v-navigation-drawer>
      <hr>
      <!-- Card Material Design -->
      <v-layout row wrap>
        <v-flex xs12 sm6>
          <v-card>
            <v-img src="https://media.licdn.com/dms/image/C4D03AQG7-e_d-QJzhQ/profile-displayphoto-shrink_200_200/0?e=1568851200&v=beta&t=_PKUJFV5XfkxwQ6PZC5w9Wz1vJvUyreYTdtPMbM1KX0"></v-img>
            <v-card-title>
              <h2>Arthur Almeida</h2>
            </v-card-title>
            <v-card-text>
              <p>
                Profissional de TI, programador, cursando Bacharelado em Ciências da Computação pela UNINOVE. 
                Atuando na área de TI há mais de 2 anos, mais de 15 cursos e diversos certificados 
                voltados para linguagens de programação, sistemas operacionais e metodologias ágeis. 
                Estou envolvido com Desenvolvimento de Softwares e Aplicações Web.
              </p>
            </v-card-text>
            <v-card-actions>
              <v-btn color="info" flat>Ação</v-btn>
            </v-card-actions>
          </v-card>
        </v-flex>

        <v-flex xs12 sm6>
          <v-card>
            <v-img src="https://media.licdn.com/dms/image/C4D03AQG7-e_d-QJzhQ/profile-displayphoto-shrink_200_200/0?e=1568851200&v=beta&t=_PKUJFV5XfkxwQ6PZC5w9Wz1vJvUyreYTdtPMbM1KX0">
              <v-container>
                <v-layout>
                  <v-flex>
                    <span class="headline black--text">insira um texto</span>
                  </v-flex>
                </v-layout>
              </v-container>
            </v-img>
            <v-card-title>
              <h2>Arthur Almeida</h2>
            </v-card-title>
            <v-card-text>
              <p>
                Profissional de TI, programador, cursando Bacharelado em Ciências da Computação pela UNINOVE. 
                Atuando na área de TI há mais de 2 anos, mais de 15 cursos e diversos certificados 
                voltados para linguagens de programação, sistemas operacionais e metodologias ágeis. 
                Estou envolvido com Desenvolvimento de Softwares e Aplicações Web.
              </p>
            </v-card-text>
            <v-card-actions>
              <v-btn color="info" flat @click="dialog = true">Mostrar dialog</v-btn>
            </v-card-actions>
          </v-card>
        </v-flex>
      </v-layout>
      <hr>
      <!-- Dialog o Modales -->
      <v-dialog persistent v-model="dialog" width="500">
        <v-card>
          <v-card-title>Este é o titulo</v-card-title>
          <v-card-text>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nulla ab animi eveniet. Nihil reiciendis, ducimus iusto sed voluptates tempore doloribus sequi, qui asperiores fugiat voluptate, id ab mollitia error tempora!
          </v-card-text>
          <v-divider></v-divider>
          <v-card-actions>
            <v-btn @click="dialog = false">Fechar</v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </v-container>
  </v-app>
</template>

<script>
  export default {
    name: "App",
    data(){
      return{
        drawer: true,
        dialog: false
      };
    }
  };
</script>

<style>
</style>
