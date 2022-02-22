<template >
  <v-container >
     <div class="elevation-12 mt-1">
                <v-toolbar class="elevation-1  mt-1"
                  dark
                  prominent
                  src="https://neilpatel.com/br/blog/cor-para-aumentar-conversao/"
                >

                  <v-app-bar-nav-icon></v-app-bar-nav-icon>
                  <v-toolbar-title>Psicologia</v-toolbar-title>
                  <v-spacer></v-spacer>

                </v-toolbar>
          </div>
     
      <v-row align="center" justify="center"  >
          <v-col cols="12" sm="100">
            <v-card class="elevation-12 mt-1"  >
             <v-window v-model="step">
                <v-window-item :value="1">
                  <v-row>
                    <v-col cols="12" md="6">
                      <v-card-text class="mt-12">
                        <h1 
                          class="text-center "
                        >Sejaas Feliz</h1>
                        <h3
                          class="text-center  grey--text "
                        ><br>Quando me tratas mal e, desprezado,
                        Sinto que o meu valor vês com desdém,
                        Lutando contra mim, fico a teu lado
                        E, inda perjuro, provo que és um bem.
                        Conhecendo melhor meus próprios erros,
                        A te apoiar te ponho a par da história
                        De ocultas faltas, onde estou enfermo;
                        Então, ao me perder, tens toda a glória.
                        Mas lucro também tiro desse ofício:
                        Curvando sobre ti amor tamanho,
                        Mal que me faço me traz benefício,
                        </h3>
                        <br> <v-row align="center" justify="center">
                          <v-col cols="12" sm="5">
                          
                            <v-row>
                              <v-col cols="12" sm="7">
                              </v-col>
                            </v-row>
                          <v-btn color="#212121" dark block tile>Log in</v-btn>

                          </v-col>
                        </v-row>  
                      </v-card-text>
                    </v-col>
                    <v-col cols="12" md="6" class="grey darken-4 rounded-bl-xl" >
                    <div style="  text-align: center; padding: 180px 0; ">
                      <v-card-text class="white--text" >
                        <h3 class="text-center ">Não tem uma conta ainda?</h3>
                        <h6
                          class="text-center"
                        >Vamos configurar tudo para que você possa começar a criar sua primeira<br>  experiência de integração</h6>
                      </v-card-text>
                      <div class="text-center">
                        <v-btn tile outlined dark @click="step++">SIGN UP</v-btn>
                      </div>
                      </div>
                    </v-col>
                  </v-row>
                </v-window-item>
                <v-window-item :value="2">
                  <v-row >
                    <v-col cols="12" md="6" class="grey darken-4 rounded-br-xl">
                     <div style="  text-align: center; padding: 180px 0;">
                      <v-card-text class="white--text" >
                        <h3 class="text-center ">Já se inscreveu?</h3>
                        <h6
                          class="text-center"
                        >Faça login em sua conta para continuar marcando as consultas</h6>
                      </v-card-text>
                      <div class="text-center">
                        <v-btn tile outlined dark @click="step--">Log in</v-btn>
                      </div>
                      </div>
                    </v-col>

                    <v-col cols="12" md="6">
                      <v-card-text class="mt-12">
                        <h4
                          class="text-center"
                        >Inscreva-se para criar uma conta</h4>
                        <h6
                          class="text-center  grey--text "
                        >Vamos configurar tudo para que você possa começar <br>
                        a criar sua primeira experiência</h6>
                        <v-row align="center" justify="center">
                          <v-col cols="12" sm="8">
                           <v-row>
                           <v-col cols="12" sm="6">
                            <v-text-field
                            label="Nome"
                            outlined
                            dense
                            color="black"
                            autocomplete="false"
                           class="mt-4"
                          />
                           </v-col>
                           <v-col cols="12" sm="6">
                            <v-text-field
                            label="Sobrenome"
                            outlined
                            dense
                            color="black"
                            autocomplete="false"
                           class="mt-4"
                          />
                           </v-col>
                           </v-row>
                          <v-text-field
                            label="E-mail"
                            outlined
                            dense
                            color="black"
                            autocomplete="false"
                          />
                          <v-text-field
                            label="Senha"
                            outlined
                            dense
                            color="black"
                          autocomplete="false"
                           type="Senha"
                          
                          />
                            <v-row>
                              <v-col cols="12" sm="7">
                                <v-checkbox
                       
                        label="Eu aceito"
                        class="mt-n1"
                        color="black"
                      > </v-checkbox>
                              </v-col>
                              <v-col cols="12" sm="5">
                                <span class="caption grey--text ml-n10">Termos e Condições</span>
                              </v-col>
                            </v-row>
                          <v-btn color="grey darken-4 " dark block tile>Sign up</v-btn>

                          </v-col>
                        </v-row>  
                      </v-card-text>
                    </v-col>
                  </v-row>
                </v-window-item>
              </v-window>
            </v-card>
          </v-col>
      </v-row>
  </v-container>
</template>

<script>
  

  export default {
   data: () => ({
    step: 1
  }),
  props: {
    source: String
  } 

    
  }
</script>
<style scoped>
.v-application .rounded-bl-xl {
    border-bottom-left-radius: 300px !important;
}
.v-application .rounded-br-xl {
    border-bottom-right-radius: 300px !important;
}

</style>
