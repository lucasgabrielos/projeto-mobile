<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Projeto 1 – Mobile</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large"></ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-card style="padding-left: 50px;">
        <img style="max-width: 50%; margin-left: 100px;" alt="Silhouette of mountains" src="https://cdn.awsli.com.br/600x700/464/464580/produto/16610111/68c964f1e9.jpg"/>
        <ion-card-content>
          Este aplicativo foi desenvolvido como parte da aplicação da disciplina de desenvolvimento mobile.
        </ion-card-content>
      </ion-card>
      <ion-card>
        <ion-card-content>
          Contribuiram com este projeto: 
        </ion-card-content>
        <ion-list>
          <ion-item>
            <ion-avatar aria-hidden="true" slot="start">
              <img alt="" src="https://ionicframework.com/docs/img/demos/avatar.svg" />
            </ion-avatar>
            Lucas Gabriel - 01494048
          </ion-item>
          <ion-item>
            <ion-avatar aria-hidden="true" slot="start">
              <img alt="" src="https://ionicframework.com/docs/img/demos/avatar.svg" />
            </ion-avatar>
            Maria Fernanda namorada linda - 01460288
          </ion-item>
          <ion-item>
            <ion-avatar aria-hidden="true" slot="start">
              <img alt="" src="https://ionicframework.com/docs/img/demos/avatar.svg" />
            </ion-avatar>
            Roronoa Zoro - 01494048
          </ion-item>
          <ion-item>
            <ion-avatar aria-hidden="true" slot="start">
              <img alt="" src="https://ionicframework.com/docs/img/demos/avatar.svg" />
            </ion-avatar>
            Neymar Jr - 01494048
          </ion-item>
        </ion-list>
      </ion-card>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonIcon } from '@ionic/vue';
import { triangle, happyOutline } from 'ionicons/icons';
import ExploreContainer from '@/components/ExploreContainer.vue';
</script>

