<template>
    <div class="ion-margin">
        <div class="flex-col">
            
            <ion-icon :icon="umbrellaOutline" color="dark"></ion-icon>
            
            <ion-text color="dark" class="title">
                Seguros
            </ion-text> 

            <ion-text color="medium" class="xs">
                Proteção para você cuidar do que importa
            </ion-text> 

            <div class="card-segur">
                <div>
                    <svg width="22" height="22" viewBox="0 0 14 22" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true"><path d="M9 16H5V18H9V16Z" fill="#111"></path><path d="M0 4V18C0 20.2091 1.79086 22 4 22H10C12.2091 22 14 20.2091 14 18V4C14 1.79086 12.2091 0 10 0H4C1.79086 0 0 1.79086 0 4ZM4 2H10C11.1046 2 12 2.89543 12 4V18C12 19.1046 11.1046 20 10 20H4C2.89543 20 2 19.1046 2 18V4C2 2.89543 2.89543 2 4 2Z" fill="#111"></path></svg>
                    <ion-text color="dark">
                        Seguro de vida
                    </ion-text>
                </div>
                
                <ion-text class="conhecer">
                    Conhecer
                </ion-text>

            </div>
            <div class="card-segur">
                <div>
                    <ion-icon :icon="heartOutline" color="dark"></ion-icon>
                    <ion-text color="dark">
                        Seguro celular
                    </ion-text>
                </div>
                <ion-text class="conhecer">
                    Conhecer
                </ion-text>
            </div>
            
        </div>
    </div>
</template>
<script>
import { umbrellaOutline, heartOutline } from 'ionicons/icons';
// Import Swiper Vue.js components
import { IonText,  IonIcon } from '@ionic/vue';

// import required modules

export default {
  name: 'SegurosComponent',
  components: {
    IonText,
    IonIcon
  },
  
  setup() {
      return { umbrellaOutline, heartOutline }
  },
};
</script>
<style scoped>
    ion-icon{
        width: 23px;
        height: 23px;
    }
    .title{
        font-size: 20px;
        font-weight: bold;
        margin: 15px 0;
    }
    .flex-col{
        display: flex;
        flex-direction: column;
    }
    
    .card-segur{
        margin-top: 15px;
        padding: 15px;
        display: flex;
        align-items: center;
        background: #f0f1f5;
        border-radius: 8px;
        display: flex;
        justify-content: space-between;
    }
    .card-segur ion-text{
       margin-left: 5%;
       font-size: 15px;
       font-weight: bold;
    }
    .card-segur .conhecer{
        color: #9a3cd9;
    }
    .card-segur div{
        width:60%;
        display: flex;
        align-items: center;
    }
    .xs{
        font-size: 14px;
    }
</style>