<template>
    <page>

        <ion-header :translucent="true">
            <ion-toolbar color="tertiary">
                <ion-buttons slot="start">
                    <ion-back-button></ion-back-button>
                </ion-buttons>
                <ion-title color="danger">การส่งของ
                </ion-title>
                <ion-icon color="danger" slot="end" size="large" :src="require('../assets/icon/location-outline.svg')"></ion-icon>
            </ion-toolbar>
        </ion-header>

        <br />

        <ion-content>
            <ion-card color="tertiary">
                <ion-card-content>
                    <ion-card-header>
                        <ion-card-title>สร้างที่อยู่ของคุณ</ion-card-title>
                        <ion-card-subtitle style="margin-top: 10px; margin-bottom: 10px;">
                            สร้างที่อยู่ของคุณเพื่อเอาไปใช้ในส่วนต่างๆ ภายในแอพพลิเคชัน</ion-card-subtitle>
                    </ion-card-header>

                    <ion-button expand="full">
                        สร้างที่อยู่
                    </ion-button>
                </ion-card-content>
            </ion-card>

            <br />

            <ion-card>

                <ion-card-content>
                    <ion-text> ที่อยู่ที่ส่งของ </ion-text>
                </ion-card-content>

                <ion-list>
                    <ion-item color="tertiary">
                        <ion-icon color="danger" :src="require('../assets/icon/receipt-outline.svg')"></ion-icon>
                        <ion-label style="padding-left: 20px;">
                            ที่อยู่ 1
                            <p>
                                <ion-text color="medium">ทำทำไม</ion-text>
                            </p>
                        </ion-label>
                        <ion-note button style="font-size: 15px; padding-top:15%;">
                            เปลี่ยน
                        </ion-note>
                    </ion-item>
                </ion-list>

                <ion-card-content>
                    <ion-text> ที่อยู่ที่เคยสร้างไว้ </ion-text>
                </ion-card-content>

                <ion-list>
                    <ion-item-sliding>
                        <ion-item color="tertiary" button>
                            <ion-label>
                                ที่อยู่ 1
                                <p>
                                    <ion-text color="medium">ทำทำไม</ion-text>
                                </p>
                            </ion-label>
                        </ion-item>

                        <ion-item-options side="end">
                            <ion-item-option color="danger">Delete</ion-item-option>
                        </ion-item-options>
                    </ion-item-sliding>

                    <ion-item-sliding>
                        <ion-item color="tertiary" button>
                            <ion-label>
                                ที่อยู่ 2
                                <p>
                                    <ion-text color="medium">ทดสอบดู</ion-text>
                                </p>
                            </ion-label>
                        </ion-item>

                        <ion-item-options side="end">
                            <ion-item-option color="danger">Delete</ion-item-option>
                        </ion-item-options>
                    </ion-item-sliding>

                </ion-list>
            </ion-card>
        </ion-content>

    </page>
</template>

<script>
import {
    IonCard,
    IonCardHeader,
    IonCardSubtitle,
    IonCardTitle,
    IonIcon,
    IonItem,
    IonLabel,
    IonButton,
    IonCardContent,
    IonToolbar,
    IonHeader,
    IonTitle,
    IonContent,
    IonBackButton,
    IonButtons,
    IonFab,
    IonFabButton,
    IonItemSliding,
    IonList,
    IonItemOptions,

} from '@ionic/vue';
import { warning } from 'ionicons/icons';
import { defineComponent } from 'vue';

export default defineComponent({
    components: {
        IonCard,
        IonCardHeader,
        IonCardSubtitle,
        IonCardTitle,
        IonIcon,
        // IonItem,
        // IonLabel,
        IonButton,
        IonCardContent,
        IonToolbar,
        IonHeader,
        IonTitle,
        IonContent,
        IonBackButton,
        IonButtons,
        // IonFab,
        // IonFabButton,
        IonItemSliding,
        IonList,
        IonItemOptions,
    },
    setup() {
        return { warning };
    }
});
</script>