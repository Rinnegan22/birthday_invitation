<template>
    <Head :title="title" />
    <main-layout >
        Happy Birthday Dazzle Ywain
    </main-layout>
</template>

<script setup>
import { Head, usePage } from "@inertiajs/vue3";
import { computed } from "vue";

import MainLayout from "../Layouts/MainLayout.vue";

const page = usePage();
const appName = computed(() => {
    return page.props.appName ?? "App Name";
});

const title = computed(() => {
    return `Dazzle Ywain`;
});
</script>