<template>
  <v-card class="mx-auto" width="300" height="100%">
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
          <DatePicker v-model="myvar" style="width: 180px" :date="time[0]" />
          <DatePicker style="width: 180px" :date="time[1]" />
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
  {{ time[0] }}
</template>

<script>
export default {
  data: () => ({
    myvar: undefined,
    open: ['Filters'],
    time: [
      new Date().toLocaleString().slice(0, 9),
      new Date().toLocaleString().slice(0, 9),
    ],
  }),
};
</script>
