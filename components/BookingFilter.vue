<!-- <template>
  <div class="d-flex align-center border-lg">
    <div style="width: 400px" class="d-flex align-center">
      <span>PERIODO:</span>
      <DatePicker style="padding: 0 20px" />
      <DatePicker />
      <v-date-input label="Date input"></v-date-input>
    </div>
    <div>
      <span>CABAÑA:</span>
    </div>
  </div>
</template>

<style></style> -->

<template>
  <v-card class="mx-auto" width="300">
    <v-list v-model:opened="open">
      <v-list-item
        prepend-icon="mdi-filter-multiple"
        title="Filtros"
      ></v-list-item>

      <v-list-group value="time">
        <template v-slot:activator="{ props }">
          <v-list-item
            v-bind="props"
            prepend-icon="mdi-calendar-range"
            title="Periodo"
          ></v-list-item>
        </template>

        <v-list-item>
          <DatePicker style="width: 180px" />
          <DatePicker style="width: 180px" />
        </v-list-item>
      </v-list-group>

      <v-list-group value="room">
        <template v-slot:activator="{ props }">
          <v-list-item
            v-bind="props"
            prepend-icon="mdi-bed"
            title="Cabañas"
          ></v-list-item>
        </template>

        <v-list-item>
          <template v-slot:prepend="{ isActive }">
            <v-checkbox-btn :model-value="isActive"></v-checkbox-btn>
          </template>
          <v-list-item-title>Ancestral</v-list-item-title>
        </v-list-item>

        <v-list-item>
          <template v-slot:prepend="{ isActive }">
            <v-checkbox-btn :model-value="isActive"></v-checkbox-btn>
          </template>
          <v-list-item-title>Safari</v-list-item-title>
        </v-list-item>
      </v-list-group>
    </v-list>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    open: ['Users'],
    admins: [
      ['Management', 'mdi-account-multiple-outline'],
      ['Settings', 'mdi-cog-outline'],
    ],
    cruds: [
      ['Create', 'mdi-plus-outline'],
      ['Read', 'mdi-file-outline'],
      ['Update', 'mdi-update'],
      ['Delete', 'mdi-delete'],
    ],
  }),
};
</script>
