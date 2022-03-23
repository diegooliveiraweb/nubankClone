<template>
  <div>
    <div class="ion-margin">
      <ion-text color="dark" class="title">
          Descubra mais
      </ion-text> 
    </div>
    
    <swiper
      :slidesPerView="'auto'"
      :spaceBetween="15"
      class="mySwiper"
    >

      <swiper-slide style="margin-left: 15px;">
        <ion-card>
          <ion-img :src="require('@/assets/img/marca-thumb.webp')"></ion-img>
        
          <ion-card-content>
            <ion-card-header>
              <ion-card-title>Portabilidade de salário</ion-card-title>
            </ion-card-header>
            <ion-text color="medium">Sua liberdade financeira começa com você escolhend...</ion-text>
            <div>
              <ion-button style="--background: #9a3cd9;">Conhecer</ion-button>
            </div>
            
          </ion-card-content>
        </ion-card>
      </swiper-slide>

      <swiper-slide >
        <ion-card>
          <ion-img :src="require('@/assets/img/marca-thumb.webp')"></ion-img>
        
          <ion-card-content>
            <ion-card-header>
              <ion-card-title>Indique seus amigos</ion-card-title>
            </ion-card-header>
            <ion-text color="medium">Mostre aos seus amigos como é fácil ter uma vida sem...</ion-text>
            <div>
              <ion-button style="--background: #9a3cd9;">Conhecer</ion-button>
            </div>
            
          </ion-card-content>
        </ion-card>
      </swiper-slide>

      <swiper-slide >
        <ion-card>
          <ion-img :src="require('@/assets/img/marca-thumb.webp')"></ion-img>
        
          <ion-card-content>
            <ion-card-header>
              <ion-card-title>Seguro de Celular</ion-card-title>
            </ion-card-header>
            <ion-text color="medium">Simples e com preço justo para você não perder nada da vida ...</ion-text>
            <div>
              <ion-button style="--background: #9a3cd9;">Conhecer</ion-button>
            </div>
            
          </ion-card-content>
        </ion-card>
      </swiper-slide>

    </swiper>
  </div>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";
import { IonCard, IonCardHeader, IonCardTitle, IonImg, IonText, IonButton, IonCardContent } from '@ionic/vue';

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";

// import required modules

export default {
  name: 'DescubraMaisComponent',
  components: {
    Swiper,
    SwiperSlide,
    IonCard, 
    IonCardHeader, 
    IonCardTitle, 
    IonImg,
    IonText,
    IonButton,
    IonCardContent
  }
};
</script>
<style scoped>
.title{
  font-size: 18px;
  font-weight: bold;
  margin: 15px 0;
}
.swiper {
  margin-top: 20px;
  width: 100%;
  height: 100%;
  padding-bottom:20px;
}

/* .swiper-slide {
  height: 350px;
} */

.swiper-slide {
  width: 66%;
  margin-left: 0;
}
.swiper-slide ion-text{
    font-size: 14px; 
    max-width: 96%;
}
.swiper-slide ion-text span{
    color: #9a3cd9;
}
ion-card{
  border-radius: 10px;
  --background: #f0f1f5;
  box-shadow: none;
}
ion-card-title{
  font-size: 14px; 
  font-weight: bold;
  margin-bottom: 10px;
}
ion-button{
  --border-radius:40px;
  margin-top: 10px;
  font-size: 14px;
  text-transform: none;
}

</style>