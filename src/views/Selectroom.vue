<template>
  <ion-page>
    <ion-header mode="ios">
      <ion-toolbar color="danger">
        <ion-buttons slot="start">
          <ion-back-button text=""></ion-back-button>
        </ion-buttons>
        <ion-title>Select Room</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content>
      <ion-card>
        <ion-card-content>
          <ion-card color="tertiary" class="ion-no-padding border-radius">
            <div class="ion-no-margin">
              <ion-slides>
                <ion-slide>
                  <div class="slide">
                    <img
                      src="https://t-cf.bstatic.com/xdata/images/hotel/max1024x768/161159671.jpg?k=303338a6b1b5474e670d5b6cd98ae38bc44ad3576d9743cc516964f1aee5a679&o=&hp=1"
                    />
                  </div>
                </ion-slide>

                <ion-slide>
                  <img
                    src="https://q-xx.bstatic.com/xdata/images/hotel/840x460/254757500.jpg?k=bb578979af0504039ad0f9128ae638fa15cfe603ba8433455bf2838b6fb56c83&o="
                  />
                </ion-slide>

                <ion-slide>
                  <img
                    src="https://q-xx.bstatic.com/xdata/images/hotel/840x460/161157933.jpg?k=783968aa8c11cc3b929f05565caaa5d7c8222240e8f2ec95786388667d3ec6e9&o="
                  />
                </ion-slide>

                <ion-slide>
                  <img
                    src="https://q-xx.bstatic.com/xdata/images/hotel/840x460/161160701.jpg?k=f3e9e1ca2be94cf213f12a4b21ae82a4ece902f3f0fd05632cde4877a801c6e1&o="
                  />
                </ion-slide>
              </ion-slides>

              <ion-grid>
                <ion-row>
                  <ion-col size="7">
                    <ion-label color="dark">
                      <h2><b>Rimtalay Resort Koh Larn</b></h2>
                      <h3>ริมทะเล รีสอร์ท</h3>
                    </ion-label>
                  </ion-col>
                  <ion-col size="5">
                    <ion-label>
                      <h3 class="ion-text-right">
                        <ion-text color="danger">
                          <h2>
                            2,436<small>&nbsp;THB</small><span>/ห้อง/คืน</span>
                          </h2>
                        </ion-text>
                        <ion-text color="medium"> ราคารวมภาษีแล้ว </ion-text>
                      </h3>
                    </ion-label>
                  </ion-col>
                </ion-row>
              </ion-grid>

              <ion-select
                interface="action-sheet"
                placeholder="เลือกประเภทห้องพัก"
              >
                <ion-select-option value="Standard Queen Room"
                  >Standard Queen Room</ion-select-option
                >
                <ion-select-option value="Superior Queen Room"
                  >Superior Queen Room</ion-select-option
                >
                <ion-select-option value="Blue Ocean Villa"
                  >Blue Ocean Villa</ion-select-option
                >
                <ion-select-option value="Blue Ocean"
                  >Blue Ocean</ion-select-option
                >
                <ion-select-option value="Green Ocean"
                  >Green Ocean</ion-select-option
                >
              </ion-select>

              <ion-card-content style="text-align: left">
                <ion-label color="dark">
                  <ion-icon :icon="bedOutline"></ion-icon>&nbsp;1
                  เตียงควีนไซส์<br />
                  <ion-icon :icon="wifiOutline"></ion-icon>&nbsp;ฟรี Wi-Fi<br />
                  <ion-icon :icon="fastFoodOutline"></ion-icon
                  >&nbsp;ฟรีอาหารเช้า<br />
                  &nbsp;ยกเลิกการจองได้ฟรี</ion-label
                >
              </ion-card-content>
              <ion-button
                color="danger"
                class="ion-no-margin"
                expand="full"
                routerLink="/cartedit"
                >เลือก</ion-button
              >
            </div>
          </ion-card>
        </ion-card-content>
      </ion-card>
    </ion-content>
  </ion-page>
</template>

<script>
import { defineComponent } from "vue";
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
  IonButton,
  IonButtons,
  IonBackButton,
  IonLabel,
  IonIcon,
  IonSelect,
  IonSelectOption,
  IonCard,
  IonCardContent,
  IonSlide,
  IonSlides,
  IonGrid,
  IonRow,
  IonCol,
  IonText
} from "@ionic/vue";
import { bedOutline, wifiOutline, fastFoodOutline } from "ionicons/icons";

export default defineComponent({
  name: "SelectHotel",
  components: {
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonPage,
    IonButton,
    IonButtons,
    IonBackButton,
    IonLabel,
    IonIcon,
    IonSelect,
    IonSelectOption,
    IonCard,
    IonCardContent,
    IonSlide,
    IonSlides,
    IonGrid,
    IonRow,
    IonCol,
    IonText
  },
  setup() {
    return {
      bedOutline,
      wifiOutline,
      fastFoodOutline,
    };
  },
});
</script>
<style scoped>
.cardpromo {
  height: 300px;
}

.imgpromo {
  height: 220px;
}

ion-searchbar {
  margin: auto;
  width: 100%;
  border-radius: 1px;
}
</style>