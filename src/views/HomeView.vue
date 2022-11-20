<script>
import auth from "../conexion/auth";
import Dashboard from "../components/Dashboard.vue"
import DashboardUser from "../components/DashboardUser.vue"
export default {
  name: "Home",
  components: {
    Dashboard,
    DashboardUser
  },
  computed: {
    userLogged() {
      return auth.getUserLogged();
    }
  },
};
</script>

<template>
  <main>
    <DashboardUser v-if="userLogged"/>
    <Dashboard v-if="!userLogged"/>
  </main>
</template>
