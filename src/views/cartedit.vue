<template>
  <ion-page>
    <ion-header mode="ios">
      <ion-toolbar color="danger">
        <ion-buttons slot="start">
          <ion-back-button text="" icon="chevron-back-outline"></ion-back-button>
        </ion-buttons>
        <ion-title>Payment Detail</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content class="transaction" mode="ios">
      <ion-card>
        <ion-card-content color="tertiary">
          <div>
            <ion-card color="tertiary" class="ion-no-padding border-radius">
              <ion-list>
                <ion-item lines="full" color="tertiary" class="ion-vertical">
                  <ion-label>
                    <h2><b>รายละเอียดการชำระเงิน</b></h2>
                  </ion-label>
                </ion-item>
                <ion-item lines="full" color="tertiary">
                  <ion-label>
                    <h3><b>ใส่โค้ดส่วนลด:&nbsp; </b></h3>
                  </ion-label>
                  <ion-input></ion-input>
                  <ion-chip color="danger">
                    <ion-label color="danger">ใช้</ion-label>
                  </ion-chip>
                </ion-item>
              </ion-list>

              <ion-item class="ion-no-padding" color="tertiary" lines="none">
                <ion-grid class="ion-padding">
                  <ion-row>
                    <ion-col class="ion-no-padding">
                      <ion-label color="medium">
                        <h3 class="line-height2">รวมค่าสินค้า</h3>
                      </ion-label>
                    </ion-col>
                    <ion-col class="ion-no-padding ion-text-right">
                      <ion-label color="medium">
                        <h3>
                          10,000
                          <small>THB</small>
                        </h3>
                      </ion-label>
                    </ion-col>
                  </ion-row>
                  <ion-row>
                    <ion-col class="ion-no-padding">
                      <ion-label color="medium">
                        <h3 class="line-height2">ค่าจัดส่ง</h3>
                      </ion-label>
                    </ion-col>
                    <ion-col class="ion-no-padding ion-text-right">
                      <ion-label color="medium">
                        <h3>
                          0
                          <small>THB</small>
                        </h3>
                      </ion-label>
                    </ion-col>
                  </ion-row>
                  <ion-row>
                    <ion-col class="ion-no-padding">
                      <ion-label color="medium">
                        <h3 class="line-height2">ส่วนลด</h3>
                      </ion-label>
                    </ion-col>
                    <ion-col class="ion-no-padding ion-text-right">
                      <ion-label color="medium">
                        <h3>
                          4,000
                          <small>THB</small>
                        </h3>
                      </ion-label>
                    </ion-col>
                  </ion-row>
                  <ion-row>
                    <ion-col class="ion-no-padding">
                      <ion-label color="medium">
                        <h3 class="line-height2">ราคารวมทั้งหมด</h3>
                      </ion-label>
                    </ion-col>
                    <ion-col class="ion-no-padding ion-text-right">
                      <ion-text color="danger">
                        <ion-label>
                          <h3>
                            <b>10,000
                              <small>THB</small>
                            </b>
                          </h3>
                        </ion-label>
                      </ion-text>
                    </ion-col>
                  </ion-row>
                </ion-grid>
              </ion-item>
              <ion-list class="ion-margin-top" lines="full">
                <ion-item color="tertiary" class="ion-padding-vertical">
                  <ion-grid class="ion-no-padding text-hidden">
                    <ion-label class="ion-padding-start">
                      <h3><b>รายการที่เช่า (1 รายการ)</b></h3>
                    </ion-label>
                    <ion-row class="ion-no-padding ion-align-items-left ion-padding-top">
                      <ion-col justify-content-center align-items-left size="auto"
                        class="ion-text-center ion-padding-start">
                        <img class="logo-l" :src="require('../assets/imgs/defaultshop.png')" />
                      </ion-col>

                      <ion-col class="ion-padding-start">
                        <ion-row>
                          <ion-col size="6">
                            <ion-label>
                              <h3>X1 Tesla Roadster</h3>
                            </ion-label>
                          </ion-col>
                          <ion-col size="6">
                            <ion-label>
                              <h3 class="ion-text-right">
                                <ion-text color="danger" class="line-through">
                                  14,000
                                </ion-text>
                                <small>&nbsp;THB</small>
                              </h3>
                            </ion-label>
                          </ion-col>
                        </ion-row>

                        <ion-row>
                          <ion-col size="6">
                            <ion-label color="danger">
                              <small>30 พ.ค.,12.00 น.- 1 มิ.ย.,12.00 น.</small>
                            </ion-label>
                          </ion-col>
                          <ion-col size="6">
                            <ion-label>
                              <h3 class="ion-text-right">
                                <ion-text> 10,000 </ion-text>
                                <small>&nbsp;THB</small>
                              </h3>
                            </ion-label>
                          </ion-col>
                        </ion-row>

                        <ion-row>
                          <ion-col class="ion-no-padding ion-text-right">
                            <ion-label color="medium">
                              <h3>
                                <span>ลบ</span>
                              </h3>
                            </ion-label>
                          </ion-col>
                        </ion-row>
                      </ion-col>
                    </ion-row>
                  </ion-grid>
                </ion-item>
              </ion-list>
              <ion-list>
                <ion-card-header mode="md" color="tertiary">
                  <ion-card-title style="font-size: 18px">ข้อมูลผู้ทำรายการ</ion-card-title>
                </ion-card-header>
                <ion-item lines="full" mode="ios" color="tertiary">
                  <ion-label>ใช้ข้อมูล KYC</ion-label>
                  <ion-toggle color="danger"></ion-toggle>
                </ion-item>
                <ion-item lines="full" color="tertiary">
                  <ion-select mode="ios" class="ion-no-padding ion-padding-end ion-select-full" okText="ตกลง"
                    cancelText="ยกเลิก" interface="action-sheet" placeholder="คำนำหน้า">
                    <ion-select-option value="male">นาย (Mr.)</ion-select-option>
                    <ion-select-option value="female1">นางสาว (Ms.)</ion-select-option>
                    <ion-select-option value="female2">นาง (Mrs.)</ion-select-option>
                  </ion-select>
                </ion-item>
                <ion-item lines="full" color="tertiary">
                  <ion-input placeholder="ชื่อ surname " type="text"></ion-input>
                </ion-item>
                <ion-item lines="full" color="tertiary">
                  <ion-input placeholder="นามสกุล lastname " type="text"></ion-input>
                </ion-item>
                <ion-item lines="full " color="tertiary ">
                  <ion-input placeholder="เบอร์ติดต่อ tel " type="tel "></ion-input>
                </ion-item>
                <ion-item lines="full " color="tertiary ">
                  <ion-input placeholder="สัญชาติ nationality " type="text"></ion-input>
                </ion-item>
                <ion-accordion-group color="tertiary" mode="ios">
                  <ion-accordion value="start" color="tertiary" toggleIconSlot="start"
                    style="border-bottom: 1px solid #e0e0e0;">
                    <ion-item slot="header" color="tertiary">
                      <ion-label>วันเดือนปีเกิด birthdate</ion-label>
                      <ion-note slot="end">{{ date0 }}</ion-note>
                    </ion-item>
                    <ion-datetime id="datetime" slot="content" locale="th-TH" @ionChange="formatDate0($event)"
                      display-format="YYYY-MM-DD"></ion-datetime>
                  </ion-accordion>
                </ion-accordion-group>
              </ion-list>

              <ion-row>
                <ion-col class="ion-no-padding ion-no-margin" size="7">
                  <ion-item lines="full" color="tertiary">
                    <ion-checkbox mode="md" color="primary" slot="start"></ion-checkbox>
                    <ion-label style="font-size: 15px">
                      ฉันได้อ่านและยอมรับ
                    </ion-label>
                  </ion-item>
                </ion-col>

                <ion-col class="ion-no-padding ion-no-margin" size="5">
                  <ion-item lines="full" color="tertiary" class="ion-no-padding ion-no-margin">
                    <ion-chip color="danger" slot="end">
                      <ion-label color="primary" @click="showData()">เงื่อนไขข้อตกลง</ion-label>
                    </ion-chip>
                  </ion-item>
                </ion-col>
              </ion-row>

              <br>
              <ion-button color="danger" class="ion-no-margin" expand="full" routerLink="/CartCheckOut">ดำเนินการต่อ
              </ion-button>
            </ion-card>
          </div>
        </ion-card-content>
      </ion-card>

      <ion-modal :is-open="modelHandle" mode="ios" ref="modal" trigger="open-modal"
        :presenting-element="$parent.$refs.ionRouterOutlet">
        <ion-header>
          <ion-toolbar style="box-shadow: none;">
            <ion-title>เงื่อนไขข้อตกลง</ion-title>
            <ion-buttons slot="end">
              <ion-button @click="hideData()">ปิด</ion-button>
            </ion-buttons>
          </ion-toolbar>
        </ion-header>
        <ion-content class="ion-padding" style="text-align: center;">
          <div style="width: 100%; margin-bottom: 1rem; margin-top: 1rem;">
          <img
            :src="require('../assets/imgs/app-development.png')"
            style="height:100px; border-radius: 50%;" />
          </div>
          <ion-note>
            ข้อมูลที่คุณกรอกนี้จะถูกใช้เพียงเพื่อยืนยันตัวตนและถูกส่งให้กับบริษัทที่เกียวข้อง
            ซึ่งจะถูกเก็บเป็นความลับ<br />
            (The information you provide about the details is solely to verify your identity and refer to the relevant
            companies.)
          </ion-note>
        </ion-content>
      </ion-modal>
    </ion-content>
  </ion-page>
</template>

<script>
import {
  IonContent,
  IonHeader,
  IonPage,
  IonTitle,
  IonToolbar,
  IonBackButton,
  IonButtons,
  IonAccordion,
  IonAccordionGroup,
  IonButton,
  IonCard,
  IonCardHeader,
  IonCardTitle,
  IonCardContent,
  IonCheckbox,
  IonItem,
  IonSelect,
  IonLabel,
  IonCol,
  IonRow,
  IonNote,
  IonInput,
  IonDatetime,
  IonSelectOption,
  IonToggle,
  IonModal,
  IonList,
  IonGrid,
  IonText,
  IonChip
} from '@ionic/vue';
import { defineComponent } from 'vue';
import moment from 'moment';
export default defineComponent({
  name: 'HomePage',
  components: {
    IonContent,
    IonHeader,
    IonPage,
    IonTitle,
    IonToolbar,
    IonBackButton,
    IonButtons,
    IonAccordion,
    IonAccordionGroup,
    IonButton,
    IonCard,
    IonInput,
    IonCardHeader,
    IonCardTitle,
    IonCardContent,
    IonCheckbox,
    IonItem,
    IonSelect,
    IonLabel,
    IonCol,
    IonRow,
    IonNote,
    IonDatetime,
    IonSelectOption,
    IonToggle,
    IonModal,
    IonList,
    IonGrid,
    IonText,
    IonChip
  },
  created() {
    this.date0 = moment().format('DD/MM/YYYY');
  },
  data() {
    return {
      driver: 'no',
      nowDate: new Date(),
      date0: "",
      modelHandle: false,
    }
  },
  methods: {
    onDriverChange(event) {
      this.driver = event.target.value;
    },
    formatDate0(event) {
      this.date0 = moment(event.target.value).format("DD/MM/YYYY");
    },
    showData() {
      this.modelHandle = true;
    },
    hideData() {
      this.modelHandle = false;
    },
  }
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
