<template>
  <swiper
    :slidesPerView="'auto'"
    :spaceBetween="2"
    class="mySwiper"
  >

    <swiper-slide style="margin-left: 15px;">
        
        <div class="icon">
            <svg alt="Logomarca do Pix" width="22" height="22" viewBox="0 0 30 30" fill="#111" xmlns="http://www.w3.org/2000/svg"><path fill="#111" d="M6.52642 22.923C7.62539 22.923 8.68209 22.5059 9.48518 21.7133L13.7545 17.5C14.0504 17.208 14.5577 17.208 14.8958 17.5L19.2068 21.7548C20.0099 22.5474 21.0666 22.9648 22.1656 22.9648H23.0109L17.6007 28.3042C15.91 29.9728 13.1626 29.9728 11.4719 28.3042L6.01953 22.923H6.52642Z" ></path><path fill="#111" d="M22.123 7.98839C21.0241 7.98839 19.9674 8.40571 19.1643 9.1983L14.8528 13.4531C14.557 13.7451 14.0497 13.7451 13.7115 13.4531L9.44262 9.23985C8.63953 8.44726 7.58283 8.03015 6.48386 8.03015H5.97656L11.4293 2.64892C13.12 0.980308 15.8674 0.980308 17.5582 2.64892L22.9684 7.98839H22.123Z" class="Path-sc-1qfmzwb-0 iybqsl"></path><path d="M1.49616 12.41L4.75087 9.19801H6.5258C7.28662 9.19801 8.04761 9.49001 8.5971 10.0323L12.866 14.2454C13.2464 14.6208 13.7961 14.8296 14.3033 14.8296C14.8105 14.8296 15.3601 14.6208 15.7406 14.2454L20.0516 9.99056C20.601 9.44826 21.362 9.15625 22.1229 9.15625H24.2363L27.491 12.3682C29.1817 14.0368 29.1817 16.7483 27.491 18.4169L24.2363 21.6291H22.1229C21.362 21.6291 20.601 21.3371 20.0516 20.7948L15.7406 16.5397C14.9797 15.7889 13.627 15.7889 12.8239 16.5397L8.555 20.753C8.00551 21.2953 7.24452 21.5873 6.4837 21.5873H4.70836L1.45364 18.3754C-0.194813 16.7902 -0.194565 14.0786 1.49616 12.41Z" class="Path-sc-1qfmzwb-0 iybqsl"></path></svg>
        </div>
        <ion-text color="dark">
            Área Pix
        </ion-text> 

    </swiper-slide>

    <swiper-slide>
        
        <div class="icon">
            <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 16 16"><path fill="#111" d="M0 3h1v10H0V3zM8 3h2v10H8V3zM11 3h1v10h-1V3zM13 3h1v10h-1V3zM15 3h1v10h-1V3zM2 3h3v10H2V3zM6 3h1v10H6V3z" class="color444 svgShape"></path></svg>
        </div>
        <ion-text color="dark">
            Pagar
        </ion-text> 

    </swiper-slide>

    <swiper-slide>
        
        <div class="icon">
           <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 16 16">
                <path d="M8 10a2 2 0 1 0 0-4 2 2 0 0 0 0 4z"/>
                <path d="M0 4a1 1 0 0 1 1-1h14a1 1 0 0 1 1 1v8a1 1 0 0 1-1 1H1a1 1 0 0 1-1-1V4zm3 0a2 2 0 0 1-2 2v4a2 2 0 0 1 2 2h10a2 2 0 0 1 2-2V6a2 2 0 0 1-2-2H3z"/>
            </svg>
        </div>
        <ion-text color="dark">
            Transferir
        </ion-text> 

    </swiper-slide>

    <swiper-slide>
        
        <div class="icon">
           <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" fill="currentColor" class="bi bi-cash-coin" viewBox="0 0 16 16">
                <path fill-rule="evenodd" d="M11 15a4 4 0 1 0 0-8 4 4 0 0 0 0 8zm5-4a5 5 0 1 1-10 0 5 5 0 0 1 10 0z"/>
                <path d="M9.438 11.944c.047.596.518 1.06 1.363 1.116v.44h.375v-.443c.875-.061 1.386-.529 1.386-1.207 0-.618-.39-.936-1.09-1.1l-.296-.07v-1.2c.376.043.614.248.671.532h.658c-.047-.575-.54-1.024-1.329-1.073V8.5h-.375v.45c-.747.073-1.255.522-1.255 1.158 0 .562.378.92 1.007 1.066l.248.061v1.272c-.384-.058-.639-.27-.696-.563h-.668zm1.36-1.354c-.369-.085-.569-.26-.569-.522 0-.294.216-.514.572-.578v1.1h-.003zm.432.746c.449.104.655.272.655.569 0 .339-.257.571-.709.614v-1.195l.054.012z"/>
                <path d="M1 0a1 1 0 0 0-1 1v8a1 1 0 0 0 1 1h4.083c.058-.344.145-.678.258-1H3a2 2 0 0 0-2-2V3a2 2 0 0 0 2-2h10a2 2 0 0 0 2 2v3.528c.38.34.717.728 1 1.154V1a1 1 0 0 0-1-1H1z"/>
                <path d="M9.998 5.083 10 5a2 2 0 1 0-3.132 1.65 5.982 5.982 0 0 1 3.13-1.567z"/>
            </svg>
        </div>
        <ion-text color="dark">
            Depositar
        </ion-text>

    </swiper-slide>

    <swiper-slide>
        
        <div class="icon">
            <svg width="22" height="22" viewBox="0 0 14 22" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true"><path d="M9 16H5V18H9V16Z" fill="#111"></path><path d="M0 4V18C0 20.2091 1.79086 22 4 22H10C12.2091 22 14 20.2091 14 18V4C14 1.79086 12.2091 0 10 0H4C1.79086 0 0 1.79086 0 4ZM4 2H10C11.1046 2 12 2.89543 12 4V18C12 19.1046 11.1046 20 10 20H4C2.89543 20 2 19.1046 2 18V4C2 2.89543 2.89543 2 4 2Z" fill="#111"></path></svg>
        </div>
        <ion-text color="dark">
            Recarga de celular
        </ion-text>

    </swiper-slide>

    <swiper-slide style="margin-left: 15px;">
        
        <div class="icon">
            <svg alt="Logomarca do Pix" width="22" height="22" viewBox="0 0 30 30" fill="#111" xmlns="http://www.w3.org/2000/svg"><path fill="#111" d="M6.52642 22.923C7.62539 22.923 8.68209 22.5059 9.48518 21.7133L13.7545 17.5C14.0504 17.208 14.5577 17.208 14.8958 17.5L19.2068 21.7548C20.0099 22.5474 21.0666 22.9648 22.1656 22.9648H23.0109L17.6007 28.3042C15.91 29.9728 13.1626 29.9728 11.4719 28.3042L6.01953 22.923H6.52642Z" ></path><path fill="#111" d="M22.123 7.98839C21.0241 7.98839 19.9674 8.40571 19.1643 9.1983L14.8528 13.4531C14.557 13.7451 14.0497 13.7451 13.7115 13.4531L9.44262 9.23985C8.63953 8.44726 7.58283 8.03015 6.48386 8.03015H5.97656L11.4293 2.64892C13.12 0.980308 15.8674 0.980308 17.5582 2.64892L22.9684 7.98839H22.123Z" class="Path-sc-1qfmzwb-0 iybqsl"></path><path d="M1.49616 12.41L4.75087 9.19801H6.5258C7.28662 9.19801 8.04761 9.49001 8.5971 10.0323L12.866 14.2454C13.2464 14.6208 13.7961 14.8296 14.3033 14.8296C14.8105 14.8296 15.3601 14.6208 15.7406 14.2454L20.0516 9.99056C20.601 9.44826 21.362 9.15625 22.1229 9.15625H24.2363L27.491 12.3682C29.1817 14.0368 29.1817 16.7483 27.491 18.4169L24.2363 21.6291H22.1229C21.362 21.6291 20.601 21.3371 20.0516 20.7948L15.7406 16.5397C14.9797 15.7889 13.627 15.7889 12.8239 16.5397L8.555 20.753C8.00551 21.2953 7.24452 21.5873 6.4837 21.5873H4.70836L1.45364 18.3754C-0.194813 16.7902 -0.194565 14.0786 1.49616 12.41Z" class="Path-sc-1qfmzwb-0 iybqsl"></path></svg>
        </div>
        <ion-text color="dark">
            Área Pix
        </ion-text> 

    </swiper-slide>

    <swiper-slide>
        
        <div class="icon">
            <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 16 16"><path fill="#111" d="M0 3h1v10H0V3zM8 3h2v10H8V3zM11 3h1v10h-1V3zM13 3h1v10h-1V3zM15 3h1v10h-1V3zM2 3h3v10H2V3zM6 3h1v10H6V3z" class="color444 svgShape"></path></svg>
        </div>
        <ion-text color="dark">
            Pagar
        </ion-text> 

    </swiper-slide>

    <swiper-slide>
        
        <div class="icon">
           <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" viewBox="0 0 16 16">
                <path d="M8 10a2 2 0 1 0 0-4 2 2 0 0 0 0 4z"/>
                <path d="M0 4a1 1 0 0 1 1-1h14a1 1 0 0 1 1 1v8a1 1 0 0 1-1 1H1a1 1 0 0 1-1-1V4zm3 0a2 2 0 0 1-2 2v4a2 2 0 0 1 2 2h10a2 2 0 0 1 2-2V6a2 2 0 0 1-2-2H3z"/>
            </svg>
        </div>
        <ion-text color="dark">
            Transferir
        </ion-text> 

    </swiper-slide>

    <swiper-slide>
        
        <div class="icon">
           <svg xmlns="http://www.w3.org/2000/svg" width="22" height="22" fill="currentColor" class="bi bi-cash-coin" viewBox="0 0 16 16">
                <path fill-rule="evenodd" d="M11 15a4 4 0 1 0 0-8 4 4 0 0 0 0 8zm5-4a5 5 0 1 1-10 0 5 5 0 0 1 10 0z"/>
                <path d="M9.438 11.944c.047.596.518 1.06 1.363 1.116v.44h.375v-.443c.875-.061 1.386-.529 1.386-1.207 0-.618-.39-.936-1.09-1.1l-.296-.07v-1.2c.376.043.614.248.671.532h.658c-.047-.575-.54-1.024-1.329-1.073V8.5h-.375v.45c-.747.073-1.255.522-1.255 1.158 0 .562.378.92 1.007 1.066l.248.061v1.272c-.384-.058-.639-.27-.696-.563h-.668zm1.36-1.354c-.369-.085-.569-.26-.569-.522 0-.294.216-.514.572-.578v1.1h-.003zm.432.746c.449.104.655.272.655.569 0 .339-.257.571-.709.614v-1.195l.054.012z"/>
                <path d="M1 0a1 1 0 0 0-1 1v8a1 1 0 0 0 1 1h4.083c.058-.344.145-.678.258-1H3a2 2 0 0 0-2-2V3a2 2 0 0 0 2-2h10a2 2 0 0 0 2 2v3.528c.38.34.717.728 1 1.154V1a1 1 0 0 0-1-1H1z"/>
                <path d="M9.998 5.083 10 5a2 2 0 1 0-3.132 1.65 5.982 5.982 0 0 1 3.13-1.567z"/>
            </svg>
        </div>
        <ion-text color="dark">
            Depositar
        </ion-text>

    </swiper-slide>

    <swiper-slide>
        
        <div class="icon">
            <svg width="22" height="22" viewBox="0 0 14 22" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true"><path d="M9 16H5V18H9V16Z" fill="#111"></path><path d="M0 4V18C0 20.2091 1.79086 22 4 22H10C12.2091 22 14 20.2091 14 18V4C14 1.79086 12.2091 0 10 0H4C1.79086 0 0 1.79086 0 4ZM4 2H10C11.1046 2 12 2.89543 12 4V18C12 19.1046 11.1046 20 10 20H4C2.89543 20 2 19.1046 2 18V4C2 2.89543 2.89543 2 4 2Z" fill="#111"></path></svg>
        </div>
        <ion-text color="dark">
            Recarga de celular
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
  name: 'AreaPixComponent',
  components: {
    Swiper,
    SwiperSlide,
    IonText
  }
};
</script>
<style scoped>
.icon{
    width: 70px;
    height: 70px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    background: #f0f1f5;
}
.swiper {
  margin-top: 30px;
  width: 100%;
  height: 100%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;

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
  width: 20%;
  margin-left: 0;
}
.swiper-slide ion-text{
    font-size: 14px;
    font-weight: bold;
    margin-top: 10px;
}
</style>