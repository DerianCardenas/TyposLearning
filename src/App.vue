<script>
import auth from "@/conexion/auth";
import { RouterLink, RouterView } from 'vue-router'
import CabeceraVue from './components/Cabecera.vue'
import CabeceraUser from './components/CabeceraUser.vue'
export default {
  name: "App",
  components: {
    CabeceraVue: CabeceraVue,
    CabeceraUser:CabeceraUser,
  },
  computed: {
    userLogged() {
      return auth.getUserLogged();
    }
  },
};
</script>

<template>
  <header class="cont-cabecera">
      <CabeceraVue v-if="!userLogged"/>
      <CabeceraUser v-if="userLogged"/>
  </header>
  <RouterView />
</template>

<style scoped>
.cont-cabecera{
  background-color:#FFFFFF;
  margin:0;
  padding:0;
  width: 100%;
}
</style>
