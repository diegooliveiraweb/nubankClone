<template>
  <ion-page>
    
    <ion-content :fullscreen="true">
      <StartComponentVue v-if="init" />
      <HomeComponent v-else />
    </ion-content>

  </ion-page>
</template>

<script>
import { StatusBar } from "@capacitor/status-bar"; 
import { IonContent, IonPage } from '@ionic/vue';
import StartComponentVue from '../components/StartComponent.vue';
import HomeComponent from '../components/HomeComponent.vue';

export default {
  name: 'HomePage',
  data() {
    return {
      init: true
    }
  },
  components: {
    IonPage,
    IonContent,
    StartComponentVue,
    HomeComponent
  },
  mounted() {
    StatusBar.setBackgroundColor({
        color: '#820ad1'
    });

    setTimeout(() => {
      this.init = false;
    }, 4000);
  },
};
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
