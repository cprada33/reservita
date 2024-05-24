<template>
  <div class="d-flex mx-13">
    <div class="d-flex align-center">
      <v-app-bar-nav-icon
        variant="text"
        @click.stop="drawer = !drawer"
      ></v-app-bar-nav-icon>
      <v-spacer></v-spacer>

      <v-navigation-drawer
        v-model="drawer"
        :location="$vuetify.display.mobile ? 'bottom' : undefined"
        temporary
      >
        <v-list-item
          v-for="route in routes"
          :to="route.route"
          :title="route.name"
          :active="false"
        ></v-list-item>
      </v-navigation-drawer>
    </div>
    <div class="v-col-3">
      <img
        src="https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fmainlogo.png?alt=media&token=cc3fd5fc-a5a3-4ad8-9fee-a51237bce3da"
        alt="logo"
        style="width: 95%"
      />
    </div>
    <div class="d-flex v-col-auto justify-space-evenly v-col-9 pa-0">
      <v-list-item
        v-for="route in routes"
        :to="route.route"
        :title="route.name"
        :active="false"
      ></v-list-item>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
    group: null,
    items: [
      {
        title: 'Foo',
        value: 'foo',
      },
      {
        title: 'Bar',
        value: 'bar',
      },
      {
        title: 'Fizz',
        value: 'fizz',
      },
      {
        title: 'Buzz',
        value: 'buzz',
      },
    ],
    routes: [
      {
        name: 'Inicio',
        route: '/',
      },
      {
        name: 'Actividades',
        route: '/actividades',
      },
      {
        name: 'Cabañas',
        route: '/cabanas',
      },
      {
        name: '¿Quienes somos?',
        route: '/somos',
      },
      {
        name: 'Contacto',
        route: '/contacto',
      },
      {
        name: 'Mi reserva',
        route: '/mireserva',
      },
    ],
  }),

  watch: {
    group() {
      this.drawer = false;
    },
  },
};
</script>
