<template>
    <ion-tabs>
        <!-- Router Outlet -->
        <ion-router-outlet></ion-router-outlet>

        <!-- Tab Bar -->
        <ion-tab-bar slot="bottom">
            <!-- Tab Home -->
            <ion-tab-button tab="home" href="/home" layout="icon-top">
                <ion-icon :icon="home"></ion-icon>
                <ion-label>Home</ion-label>
            </ion-tab-button>

            <!-- Tab Profile -->
            <ion-tab-button tab="profile" href="/profile" layout="icon-top">
                <ion-icon :icon="person"></ion-icon>
                <ion-label>Profile</ion-label>
            </ion-tab-button>
        </ion-tab-bar>
    </ion-tabs>
</template>

<script setup lang="ts">
    import {
        IonTabs,
        IonRouterOutlet,
        IonTabBar,
        IonTabButton,
        IonIcon,
        IonLabel,
    } from "@ionic/vue";
    import { home, person } from "ionicons/icons";
</script>

<style scoped>
    ion-tab-bar {
        --background: #ffffff;
        --color-selected: #3880ff;
        --color: #8c8c8c;
    }
</style>
