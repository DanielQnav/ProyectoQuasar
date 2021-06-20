<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated class="bg-blue text-white">
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="toggleLeftDrawer"
        />

        <q-toolbar-title> Encabezado</q-toolbar-title>
       <div>Version Quasar{{ $q.version }}</div>
      </q-toolbar>
    </q-header>

    <q-drawer
      v-model="leftDrawerOpen"
      side="left"
      show-if-above
      bordered
      class="bg-grey-1"
    >
      <q-list class="q-pa-md bg-blue text-center">
        <q-item-label header class="text-dark">
          Rutas de Acceso:
        </q-item-label>

        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
        <div class="col-12 q-pa-sm">
          <q-btn
            to="/"
            color="white"
            text-color="dark"
            glossy
            size="35px"
            round
            unelevated
            icon="home"
          />
        </div>
        <div class="col-12 q-pa-sm">
          <q-btn
            to="/page1"
            color="white"
            text-color="dark"
            glossy
            size="35px"
            round
            unelevated
            icon="devices"
          />
        </div>
        <div class="col-12 q-pa-sm">
          <q-btn
            to="/page2"
            class="q-btn"
            color="white"
            text-color="dark"
            glossy
            size="35px"
            round
            unelevated
            icon="design_services"
          />
        </div>
        <div class="col-12 q-pa-sm">
          <q-btn
            to="/form"
            class="q-btn"
            color="white"
            text-color="dark"
            glossy
            size="35px"
            round
            unelevated
            icon="contact_mail"
          />
        </div>
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import EssentialLink from "components/EssentialLink.vue";

const linksList = [
  {
    title: "Daniel Quintana",
    caption: "Proyecto de programador",
    icon: "dashboard",
    link: "https://github.com/DanielQnav",
  },
];

import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "MainLayout",

  components: {
    EssentialLink,
  },

  setup() {
    const leftDrawerOpen = ref(false);

    return {
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },
    };
  },
});
</script>

<style></style>
