<template>
  <swiper
    :slidesPerView="'auto'"
    :spaceBetween="15"
    class="mySwiper"
  >

    <swiper-slide style="margin-left: 15px;">
        <ion-text color="dark">
            Tem <span>SHOPPING</span> no seu bank. Conheça agora.
        </ion-text>

    </swiper-slide>

    <swiper-slide>
        <ion-text color="dark">
            Seu <span>informe de rendimentos</span> 2021 já está disponível.
        </ion-text>

    </swiper-slide>

    <swiper-slide>
        <ion-text color="dark">
            Conheça <span>Nubank Vida:</span> um seguro simples e que cabe no ...
        </ion-text>

    </swiper-slide>

    <swiper-slide>
        <ion-text color="dark">
            Salve seus amidos da burocracia. <span>Faça um convite ...</span>
        </ion-text>

    </swiper-slide>

  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";
import { IonText } from '@ionic/vue';

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";

// import required modules

export default {
  name: 'CardsInfoComponent',
  components: {
    Swiper,
    SwiperSlide,
    IonText
  }
};
</script>
<style scoped>

.swiper {
  margin-top: 20px;
  width: 100%;
  height: 100%;
}

.swiper-slide {
  font-size: 18px;
  background: #f0f1f5;
  padding: 23px;
  border-radius: 15px;
  height: 90px;

  /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  flex-direction: column;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;
}

.swiper-slide {
  width: 65%;
  margin-left: 0;
}
.swiper-slide ion-text{
    font-size: 13px; 
    max-width: 96%;
}
.swiper-slide ion-text span{
    color: #9a3cd9;
}
</style>