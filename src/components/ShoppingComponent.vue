<template>
    <div class="shopping">
        <div class="ion-margin">
            <div>
                <svg xmlns="http://www.w3.org/2000/svg" width="23" height="23" viewBox="0 0 24 24"><g fill="none" fill-rule="evenodd" stroke="#200E32" stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" transform="translate(2.5 1.5)"><path d="M14.01373 20.0000001L5.66590392 20.0000001C2.59954235 20.0000001.247139589 18.8924486.915331812 14.4347827L1.69336385 8.39359272C2.10526317 6.16933642 3.52402748 5.31807783 4.76887874 5.31807783L14.9473685 5.31807783C16.2105264 5.31807783 17.5469108 6.23340964 18.0228834 8.39359272L18.8009154 14.4347827C19.3684211 18.3890161 17.0800916 20.0000001 14.01373 20.0000001zM14.1510298 5.09839819C14.1510298 2.71232585 12.216736.7779932 9.83066366.7779932L9.83066366.7779932C8.68166274.773163349 7.57805185 1.22619323 6.76386233 2.03694736 5.9496728 2.84770148 5.49199087 3.94938696 5.49199087 5.09839819L5.49199087 5.09839819"/><line x1="12.796" x2="12.751" y1="9.602" y2="9.602"/><line x1="6.966" x2="6.92" y1="9.602" y2="9.602"/></g></svg>
            </div>
            <ion-grid>
                <ion-row class="ion-justify-content-between">
                    <ion-text color="dark" class="title">
                        Shopping
                    </ion-text> 
                    <ion-icon :icon="chevronForwardOutline" color="medium" class="conta"></ion-icon>
                
                </ion-row>
                    <ion-text color="medium" class="xs">
                    Vantagens exclusivas das nossas marcas preferidas
                </ion-text>              
            </ion-grid>
        </div>
    </div>
</template>
<script>
import { IonGrid, IonRow, IonText, IonIcon } from '@ionic/vue';
import { chevronForwardOutline } from 'ionicons/icons';
export default {
   name: 'ShoppingComponent',
   components:{
       IonGrid, IonRow, IonText, IonIcon
   },
   setup() {
       return { chevronForwardOutline }
   }
}
</script>
<style scoped>
    .shopping{
        border-top: 2.5px solid #f0f1f5;
        border-bottom: 2.5px solid #f0f1f5;
        margin-top: 25px;
    }
    .shopping ion-text {margin: 13px 0;}
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