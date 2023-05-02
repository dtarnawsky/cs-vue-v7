<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Blank</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Blank</ion-title>
        </ion-toolbar>
      </ion-header>

      <div id="container">
        <ion-button id="open-toast">Open Toast</ion-button>
  <ion-toast trigger="open-toast" aria-label="Hello Global World!" message="Hello World!" :duration="3000" :icon="globe"></ion-toast>      
</div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonButton, IonToast, IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import { globe } from 'ionicons/icons';
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
