<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Tienda Online</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 1</ion-title>
        </ion-toolbar>
      </ion-header>
      <div id="login-form">
          <InputComponent id="user" name="Nombre" label="Nombre: " />
          <InputComponent type="number" id="tel" name="Celular" label="Celular: " />
          <InputComponent type="email" id="email" name="correo" label="Email: " />
          <InputComponent type="date" id="fecha" name="Fecha_de_Nacimiento" />
          

          <br />

          <ButtonComponent id="consult" value="Consultar" fill="outline" />
          <ButtonComponent id="save" value="Agregar" fill="outline" color="success" />
          <ButtonComponent id="update" value="Modificar" fill="outline" color="warning" />
          <ButtonComponent id="delete" value="Eliminar" fill="outline" color="danger" />
        
        </div>
      
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar,IonButton, IonTitle, IonContent } from '@ionic/vue';
import ExploreContainer from '@/components/ExploreContainer.vue';
import ButtonComponent from '@/components/ButtonComponent.vue';
import InputComponent from '@/components/InputComponent.vue'
</script>
<style scoped>
#login-form {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 90vh; /* Usar altura completa de la ventana */
  padding: 20px; /* Añadir relleno para separar los elementos */
}

#login-form ion-item {
  width: 100%; /* Ajustar el ancho de los elementos de entrada */
  margin-bottom: 10px; /* Agregar espacio entre elementos */
}

#login-form ion-button {
  width: 50%; /* Ajustar el ancho de los botones */
  margin-bottom: 30px; /* Agregar espacio entre botones */
}
</style>
