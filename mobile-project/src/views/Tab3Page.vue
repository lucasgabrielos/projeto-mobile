<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Relatórios</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-card>
        <ion-card-content>
          <ion-list>
            <ion-label>Relatórios</ion-label>
            <ion-item>Senhas emitidas: {{senhasService.senhasTotal}}</ion-item>
            <ion-item>Senhas Geral: {{senhasService.senhasGeral}}</ion-item>
            <ion-item>Senhas Prioritária: {{senhasService.senhasPrior}}</ion-item>
            <ion-item>Senhas Exame: {{senhasService.senhasExame}}</ion-item>
          </ion-list>
        </ion-card-content>
      </ion-card>
    </ion-content>
  </ion-page>
</template>
<script setup lang="ts">

import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import {PasswordsService} from '../Services/passwordService';
import ExploreContainer from '@/components/ExploreContainer.vue';

const senhasService = new PasswordsService();

</script>
