<template>
  <div class="home">
    <v-container>
      <v-row justify="center" class="mt-16">
        <v-col cols="12" sm="8" class="box">
          <div>
            <h1>Desafia las expectativas de los MOBA</h1>
            <p>Épicos héroes y accion sin cesar en múltiples campos de batalla</p>
            <v-btn color="orange darken-1" @click="$router.push('/heroes')" class="text-white mt-2">Ver Héroes</v-btn>
          </div>
        </v-col>
      </v-row>
    </v-container>
    <v-alert
      class="py-5 mt-14"
      v-model="alert"
      border="start"
      style="opacity: 0.8;"
      dark
      close-label="Close Alert"
      color="purple">
      ¡Te damos la bienvenida al Nexo! ¡En este reino entre reinos, todo es posible! Elige entre decenas de héroes legendarios de todo el panteón de Blizzard, personaliza sus talentos y habilidades en medio del combate y lucha en una infinidad de campos de batalla que redefinen el género. ¡Esto no es un MOBA promedio, eso es Heroes of th Storm!
    </v-alert>
  </div>
</template>

<script>

import { defineComponent } from 'vue';

// Components


export default defineComponent({
  name: 'HomeView',

  components: {
  },
});
</script>

<style scoped>
  .home {
    background: url('../assets/img/fondo3.jpg');
    height: 100%;
    
  }
  .box{
    border: 1px solid whitesmoke;
    color: whitesmoke;
    text-align: center;
  }
</style>
