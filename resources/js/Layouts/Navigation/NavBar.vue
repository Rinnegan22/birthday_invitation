<template>
    <v-app-bar color="primary">
        <v-app-bar-nav-icon v-if="hasDrawer" @click="toggleDrawer" />

        <v-app-bar-title>
            Dazzle Ywain
        </v-app-bar-title>
        <template v-slot:append>
            <switch-theme />
        </template>
    </v-app-bar>
</template>

<script setup>
import { usePage } from "@inertiajs/vue3";

import SwitchTheme from "./Components/SwitchTheme.vue";

const props = defineProps({
    hasDrawer: {
        type: Boolean,
        default: false,
    },
    errors: Object,
    flash: Object,
    can: Array,
});


const emits = defineEmits(["toggleDrawer"]);
const toggleDrawer = () => {
    emits("toggleDrawer");
};
</script>