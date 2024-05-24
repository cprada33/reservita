<template>
  <v-row>
    <v-col cols="4">
      <img
        src="https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fbannermujer.png?alt=media&token=cfda4ded-25e4-4c97-9065-ca6f497e344c"
        alt="banner"
        style="width: 110%; height: 100%; object-fit: contain"
      />
    </v-col>
    <v-col cols="8" class="d-flex flex-column">
      <v-row>
        <v-col class="d-flex justify-center" style="font-size: 7rem"
          >BIENVENIDOS</v-col
        >
      </v-row>
      <v-row>
        <v-col
          class="d-flex justify-center align-center"
          style="font-size: 7rem"
          >A</v-col
        >
      </v-row>
      <v-row>
        <v-col class="d-flex justify-center align-start" style="font-size: 7rem"
          >LA MONTAÑA</v-col
        >
      </v-row>
      <v-row>
        <v-col
          class="d-flex justify-center align-center"
          style="font-size: 1.5rem; text-align: center"
          >Bienvenidos a esta montaña donde se rinde tributo a la herencia y
          legado ancestral, bienvenidos a nuestra casa.</v-col
        >
      </v-row>
      <v-row>
        <v-col cols="6" class="d-flex justify-end">
          <DatePicker
            v-model="dateValue"
            style="width: 230px"
            class="flex-grow-0"
          />
        </v-col>
        <v-col cols="6">
          <DatePicker style="width: 230px" v-model="dateValue" />
        </v-col>
      </v-row>
      <v-row>
        <v-col class="d-flex justify-center">
          <v-btn></v-btn>
        </v-col>
      </v-row>
    </v-col>
  </v-row>
</template>
<script lang="ts" setup>
const dateValue = ref();
</script>
