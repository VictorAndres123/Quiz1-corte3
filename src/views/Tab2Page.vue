<template>
  
    <ion-header>
      <ion-toolbar>
        <ion-title>Title</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 2</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-content class="ion-padding">
    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    <h3>Heading 3</h3>
    <h4>Heading 4</h4>
    <h5>Heading 5</h5>
    <h6>Heading 6</h6>

    <p>Here's a small text description for the content. Nothing more, nothing less.</p>
  </ion-content>
  <ion-footer>
    <ion-toolbar>
      <ion-title> Footer </ion-title>
    </ion-toolbar>
  </ion-footer>



      
    </ion-content>
</template>

<script lang="ts">
  import { IonContent, IonFooter, IonHeader, IonTitle, IonToolbar } from '@ionic/vue';
  import { defineComponent } from 'vue';

  export default defineComponent({
    components: { IonContent, IonFooter, IonHeader, IonTitle, IonToolbar },
  });
</script>