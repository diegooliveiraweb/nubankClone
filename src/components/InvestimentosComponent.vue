<template>
    <div class="invest">
        <div class="ion-margin">
            <div>
                <svg width="18" height="18" viewBox="0 0 48 48" xmlns="http://www.w3.org/2000/svg">
                    <rect width="6.478" height="20.755" x="10.429" y="27.136" rx="0.65" style=""/>
                    <rect width="6.478" height="11.852" x="0.051" y="36.016" rx="0.65" style=""/>
                    <rect width="6.478" height="29.657" x="20.788" y="18.235" rx="0.65" style=""/>
                    <rect width="6.478" height="38.559" x="31.147" y="9.333" rx="0.65" style=""/>
                    <rect width="6.478" height="47.46" x="41.525" y="0.432" rx="0.65" style=""/>
                </svg>
            </div>
            <ion-grid>
                <ion-row class="ion-justify-content-between">
                    <ion-text color="dark" class="title">
                        Investimentos
                    </ion-text> 
                    <ion-icon :icon="chevronForwardOutline" color="medium" class="conta"></ion-icon>
                
                </ion-row>
                    <ion-text color="medium" class="xs">
                    O jeito Nu de investir: sem asteriscos, linguagem fácil e a partir de R$1. Saiba mais.
                </ion-text>              
            </ion-grid>
        </div>
    </div>
</template>
<script>
import { IonGrid, IonRow, IonText, IonIcon } from '@ionic/vue';
import { chevronForwardOutline } from 'ionicons/icons';
export default {
   name: 'InvestimentosComponent',
   components:{
       IonGrid, IonRow, IonText, IonIcon
   },
   setup() {
       return { chevronForwardOutline }
   }
}
</script>
<style scoped>
    .invest{
        border-bottom: 2.5px solid #f0f1f5;
        margin-top: 25px;
    }
    .invest ion-text {margin: 13px 0;}
    .xs{
        font-size: 14px;
    }
    .title{
        font-weight: bold;
    }
    .title{
        font-size: 20px;
    }
    .fatura{
        font-size: 24px;
    }
    .flex-col{
        display: flex;
        flex-direction: column;
    }
    ion-icon{
        width: 20px;
        height: 20px;
    }
</style>