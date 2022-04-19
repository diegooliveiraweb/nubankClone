<template>
  <ion-app>
    <ion-router-outlet />
  </ion-app>
</template>

<script>
import { IonApp, IonRouterOutlet } from '@ionic/vue';

export default {
  name: 'App',
  components: {
    IonApp,
    IonRouterOutlet
  }
};
</script>
<style>
@font-face {
  font-family: GraphikRegular;
  src: url(~@/assets/fonts/GraphikRegular.otf);
}
@font-face {
  font-family: GraphikMedium;
  src: url(~@/assets/fonts/GraphikMedium.otf);
}
@font-face {
  font-family: GraphikSemibold;
  src: url(~@/assets/fonts/GraphikSemibold.otf);
}
@font-face {
  font-family: GraphikBold;
  src: url(~@/assets/fonts/GraphikBold.otf);
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: GraphikRegular, GraphikMedium, "Gotham SSm A", "Gotham SSm B", "Helvetica Neue", Helvetica, Arial, sans-serif;
}
input{
    border: none;
    background: transparent;
}
input:focus{
    outline: none;
}
</style>