<template>
  <ion-app>
    <ion-menu side="start" menu-id="first" content-id="main">
      <ion-header>
        <ion-toolbar color="primary">
          <ion-title>House Tactics</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-content>
        <ion-list>
          <ion-item>Estadisticas</ion-item>
          <ion-item>Barracones</ion-item>
          <ion-item>Party</ion-item>
          <ion-item>Misiones</ion-item>
          <ion-item>Calificaciones</ion-item>
        </ion-list>
      </ion-content>
    </ion-menu>
    <ion-router-outlet id="main"></ion-router-outlet>
  </ion-app>
</template>

<script>
import {
  IonApp,
  IonRouterOutlet,
  IonList,
  IonHeader,
  IonContent,
  IonMenu,
  IonToolbar,
  menuController,
} from "@ionic/vue";
import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
  components: {
    IonApp,
    IonRouterOutlet,
    IonList,
    IonHeader,
    IonContent,
    IonMenu,
    IonToolbar,
  },
  methods: {
    openFirst() {
      menuController.enable(true, "first");
      menuController.open("first");
    },
    openEnd() {
      menuController.open("end");
    },
    openCustom() {
      menuController.enable(true, "custom");
      menuController.open("custom");
    },
  },
});
</script>
