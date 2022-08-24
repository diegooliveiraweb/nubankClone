<template>
  <ion-page>
    <ion-content fullscreen="true" class="">
        <div class="header">
            <ion-grid>
                <ion-row class="ion-justify-content-between">
                    <ion-col size="4" class="ion-margin">
                        <div class="ion-padding user mb">
                            <ion-img :src="require('../assets/img/user.png')" class="img"></ion-img>
                        </div>
                        <ion-text color="light" class="flex">
                            Olá,&nbsp;<input type="text" v-model="name">
                        </ion-text>
                    </ion-col>
                    <ion-col size="4" class="ion-margin">
                        <ion-row class="ion-justify-content-between">
                            <ion-icon :icon="eyeOutline" color="light" @click="showHideSaldo()" v-if="showSaldo"></ion-icon>
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 256 256" class="icon"  @click="showHideSaldo()" v-else><rect width="256" height="256" fill="none"/><line x1="201.15" x2="223.96" y1="127.305" y2="166.813" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="16"/><line x1="154.182" x2="161.296" y1="149.263" y2="189.607" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="16"/><line x1="101.73" x2="94.615" y1="149.244" y2="189.594" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="16"/><line x1="54.809" x2="31.889" y1="127.272" y2="166.971" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="16"/><path fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="16" d="M31.99943,104.87509C48.81193,125.68556,79.63353,152,128,152c48.36629,0,79.18784-26.31424,96.00039-47.12468"/></svg>
                            <ion-icon :icon="helpCircleOutline" color="light"></ion-icon>   
                            <ion-icon :icon="mailUnreadOutline" color="light"></ion-icon> 
                                
                        </ion-row>
                    </ion-col>
                </ion-row>
            </ion-grid>
        </div>
        <div id="container">
            <ion-grid class="ion-margin">
                <ion-row class="ion-justify-content-between">
                    <ion-text color="dark">
                       Conta
                    </ion-text> 
                    <ion-icon :icon="chevronForwardOutline" color="medium" class="conta"></ion-icon>
                </ion-row>
                <ion-row >
                    <ion-text color="dark" class="saldo flex">
                       R$ <input type="text" v-model="saldo">
                       <Transition>
                            <span class="ocult" v-if="!showSaldo"></span>
                       </Transition>
                    </ion-text> 
                
                </ion-row>
            </ion-grid>
            <AreaPixComponent />
            <div class="ion-margin div-cartoes">
                <div class="cartoes">
                    <svg width="22" height="22" viewBox="0 0 92 92" xmlns="http://www.w3.org/2000/svg">
                        <path d="M 91.447 21.788 C 91.447 17.241 88.261 13.583 84.302 13.583 L 9.766 13.583 C 5.808 13.583 2.621 17.241 2.621 21.788 L 2.621 72.006 C 2.621 76.44 5.808 80.098 9.766 80.098 L 84.399 80.098 C 88.357 80.098 91.544 76.44 91.544 71.894 L 91.544 21.788 L 91.447 21.788 Z M 83.723 22.453 L 83.723 71.254 L 10.192 71.431 L 10.345 22.453 L 83.723 22.453 Z M 10.345 71.23 L 83.723 71.23 L 10.345 71.23 Z M 76.635 57.523 C 76.635 59.962 74.744 62.124 72.62 62.124 L 68.548 61.967 C 66.424 61.967 64.845 59.813 64.845 57.374 C 64.845 54.934 66.073 52.745 68.197 52.745 L 72.62 52.755 C 74.744 52.755 76.635 55.085 76.635 57.523 Z" style="" transform="matrix(0, -1, 1, 0, 0.241998, 93.922997)"/>
                    </svg>
                    <ion-text color="dark">
                        Meus cartões
                    </ion-text>
                
                </div>
            </div>
            <CardsInfoComponent />
            <CartaoDeCreditoComponent :showFatura="showSaldo" />
            <InvestimentosComponent />
            <SegurosComponent />
            <ShoppingComponent />
            <DescubraMaisComponent />
        
        </div>
        
    </ion-content>
  </ion-page>
</template>

<script>
import { IonContent, IonPage, IonGrid, IonRow, IonCol, IonImg, IonText, IonIcon } from '@ionic/vue';
import { eyeOutline, helpCircleOutline, mailUnreadOutline, chevronForwardOutline } from 'ionicons/icons';
import AreaPixComponent from './AreaPixComponent.vue';
import CardsInfoComponent from './CardsInfoComponent.vue';
import CartaoDeCreditoComponent from './CartaoDeCreditoComponent.vue';
import InvestimentosComponent from './InvestimentosComponent.vue';
import SegurosComponent from './SegurosComponent.vue';
import ShoppingComponent from './ShoppingComponent.vue';
import DescubraMaisComponent from './DescubraMaisComponent.vue';


export default {
  name: 'HomeComponent',
  components: {
    IonContent,
    IonPage,
    IonGrid,
    IonCol,
    IonRow,
    IonImg,
    IonText,
    IonIcon,
    AreaPixComponent,
    CardsInfoComponent,
    CartaoDeCreditoComponent,
    InvestimentosComponent,
    SegurosComponent,
    ShoppingComponent,
    DescubraMaisComponent
  },
  data() {
      return {
          showSaldo: true,
          saldo: '23.579,90',
          name: 'Diego'
      }
  },
  setup() {
      return { eyeOutline, helpCircleOutline, mailUnreadOutline, chevronForwardOutline }
  },
  methods: {
       showHideSaldo(){
          this.showSaldo = ! this.showSaldo;
      }
  },
};
</script>

<style scoped>
    .header{
        min-height: 17%;
        background-color: rgb(130, 10, 209);
    }
    .user{
       background-color: #9a3cd9; 
       border-radius: 50%;
       width: 45px;
    }
  
    .ion-padding{
        padding: 7px;
    }
    .mb{
        margin-bottom: 30px;
    }
    ion-icon {
        font-size: 26px;
        font-weight: bold;
    }
    .conta{
        font-size: 20px;
    }
    ion-text{
        font-weight: bold;
        font-size: 19px;
    }
    #container{
        margin-top: 30px;
    }
    #container .saldo{
        padding: 5px;
        font-size: 24px;
        margin-top: 18px;
        width: 70%;
        position: relative;
    }
     #container .saldo .ocult{
        position: absolute;
        width: 100%;
        left: 0;
        height: 100%;
        background: #f0f1f5;
        border-radius: 2px;
    }
    .icon{
        width: 26px;
    }
    .div-cartoes{
        margin-top: 20px;
        margin-bottom: 10px;
    }

    .cartoes{
        padding: 15px;
        display: flex;
        align-items: center;
        background: #f0f1f5;
        border-radius: 8px;
    }
    .cartoes ion-text{
       margin-left: 3%;
       font-size: 15px;
    }
    .flex{
        display: flex;
    }
    .v-enter-active,
    .v-leave-active {
        transition: opacity 0.2s ease;
    }

    .v-enter-from,
    .v-leave-to {
        opacity: 0;
    }
</style>
