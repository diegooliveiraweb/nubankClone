<template>
    <div class="cartao">
        <div class="ion-margin">
            <div>
                <svg width="22" height="22" viewBox="0 0 92 92" xmlns="http://www.w3.org/2000/svg">
                    <path d="M 91.447 21.788 C 91.447 17.241 88.261 13.583 84.302 13.583 L 9.766 13.583 C 5.808 13.583 2.621 17.241 2.621 21.788 L 2.621 72.006 C 2.621 76.44 5.808 80.098 9.766 80.098 L 84.399 80.098 C 88.357 80.098 91.544 76.44 91.544 71.894 L 91.544 21.788 L 91.447 21.788 Z M 83.723 22.453 L 83.723 71.254 L 10.192 71.431 L 10.345 22.453 L 83.723 22.453 Z M 10.345 71.23 L 83.723 71.23 L 10.345 71.23 Z M 76.635 57.523 C 76.635 59.962 74.744 62.124 72.62 62.124 L 68.548 61.967 C 66.424 61.967 64.845 59.813 64.845 57.374 C 64.845 54.934 66.073 52.745 68.197 52.745 L 72.62 52.755 C 74.744 52.755 76.635 55.085 76.635 57.523 Z" style="" transform="matrix(0, -1, 1, 0, 0.241998, 93.922997)"/>
                </svg>
            </div>
            <ion-grid>
                <ion-row class="ion-justify-content-between">
                    <div class="flex-col">
                        <ion-text color="dark" class="title">
                            Cartão de crédito
                        </ion-text> 
                        <ion-text color="medium" class="xs">
                            Fatura atual
                        </ion-text> 
                        <ion-text color="dark" class="fatura">
                            R$ <input type="text" v-model="fatura">
                            <Transition>
                                <span class="ocult" v-if="!showFatura"></span>
                            </Transition>
                        </ion-text> 
                        <ion-text color="medium" class="xs">
                            Limite disponível R$ <input type="text" v-model="limite">
                        </ion-text> 
                        
                    </div>
                    <ion-icon :icon="chevronForwardOutline" color="medium" class="conta"></ion-icon>
                </ion-row>
            </ion-grid>
        </div>
    </div>
</template>
<script>
import { IonGrid, IonRow, IonText,  IonIcon } from '@ionic/vue';
import { chevronForwardOutline } from 'ionicons/icons';


export default {
   name: 'CartaoDeCreditoComponent',
   components:{
       IonGrid, IonRow, IonText,  IonIcon
   },
   props:['showFatura'],
    setup() {

       return { chevronForwardOutline}
    },
   data() {
       return {
           fatura: '320,39',
           limite: '2.079,61'
       }
   },
   
}
</script>
<style scoped>
    .cartao{
        border-top: 2.5px solid #f0f1f5;
        border-bottom: 2.5px solid #f0f1f5;
        margin-top: 25px;
    }
    .cartao ion-text {margin: 7px 0;}
    .xs{
        font-size: 14px;
    }
    .title, .fatura{
        font-weight: bold;
    }
    .title{
        font-size: 20px;
    }
    .fatura{
        font-size: 24px;
        position: relative;
    }
    .flex-col{
        display: flex;
        flex-direction: column;
    }
    ion-icon{
        width: 20px;
        height: 20px;
    }
    .ocult{
        position: absolute;
        width: 100%;
        left: 0;
        height: 100%;
        background: #f0f1f5;
        border-radius: 2px;
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