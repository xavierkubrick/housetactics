<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-menu-button></ion-menu-button>
        </ion-buttons>
        <ion-title>
          House Tactics
        </ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content>
      <ion-card>
        <ion-card-header>
          <ion-card-subtitle>
            Tu herramienta para gestión, administración y ejecución de tácticas
            y estrategias
          </ion-card-subtitle>
        </ion-card-header>
        <ion-card-content>
          <ion-img
            src="https://i.ytimg.com/vi/fxv6lJv6Kc8/maxresdefault.jpg"
          ></ion-img>
        </ion-card-content>
      </ion-card>
      <ion-button expand="block" fill="outline">Ingresar</ion-button>
    </ion-content>
  </ion-page>
</template>

<script>
import {
  IonPage,
  IonCard,
  IonCardHeader,
  IonImg,
  IonCardContent,
  IonHeader,
  IonTitle,
  IonContent,
  IonButton,
  IonToolbar,
} from "@ionic/vue";
import { defineComponent } from "vue";

export default defineComponent({
  name: "Home",
  components: {
    IonPage,
    IonCard,
    IonCardHeader,
    IonImg,
    IonCardContent,
    IonHeader,
    IonTitle,
    IonContent,
    IonButton,
    IonToolbar,
  },
});
</script>

<style scoped>
#container {
  text-align: center;

  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;

  color: #8c8c8c;

  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
