<template>
  <v-text-field
    :date="date"
    style="width: 400px"
    variant="outlined"
    append-inner-icon="mdi-calendar-today"
    readonly
  >
    <v-menu
      activator="parent"
      location="bottom"
      :close-on-content-click="false"
    >
      <v-date-picker elevation="6"></v-date-picker>
    </v-menu>
  </v-text-field>
</template>

<script setup>
defineProps(['date']);
</script>
