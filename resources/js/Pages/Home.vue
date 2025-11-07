<template>
    <span>Hello World</span>
    <div class="text-center">
        <v-btn color="primary" append-icon="mdi-account-circle" prepend-icon="mdi-check-circle">
            <template v-slot:prepend>
                <v-icon color="success"></v-icon>
            </template>

            Button

            <template v-slot:append>
                <v-icon color="warning"></v-icon>
            </template>
        </v-btn>
    </div>
</template>
<script setup></script>
