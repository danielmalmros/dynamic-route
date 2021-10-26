<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Articles</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <strong>See in console that Settings view is mounted.</strong>
    </ion-content>
  </ion-page>
</template>
<script lang="ts">
import { defineComponent, onMounted } from "vue";
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
} from "@ionic/vue";
export default defineComponent({
  name: "Article",
  components: {
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonPage,
  },
  setup() {
    onMounted(() => {
      console.log("--- ARTICLE MOUNTED ---");
    });
  },
});
</script>
