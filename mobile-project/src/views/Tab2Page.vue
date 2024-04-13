<template>
  <ion-page>
    <ion-card>
      <ion-card-header>
        <ion-input readonly="true" label="Senha: " v-model="inputNovaSenha"></ion-input>
      </ion-card-header>
      <ion-card-content>
        <!-- Corrigindo o uso de eventos de clique -->
        <ion-button expand="block" @click="passwordService.somaGeral()">Senha Geral</ion-button>
        <ion-button expand="block" @click="passwordService.somaPrior()">Senha Prioritária</ion-button>
        <ion-button expand="block" @click="passwordService.somaExame()">Senha Exame</ion-button>
      </ion-card-content>
    </ion-card>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import { PasswordsService } from '../Services/passwordService';
import ExploreContainer from '@/components/ExploreContainer.vue';

// Declarando e inicializando a variável inputNovaSenha
let inputNovaSenha = "me calar? ninguém me cala não";

// Criando uma instância do serviço PasswordsService
const passwordService = new PasswordsService();
</script>
