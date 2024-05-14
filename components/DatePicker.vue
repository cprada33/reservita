<template>
  <v-text-field
    v-model="modelValue"
    variant="outlined"
    :append-inner-icon="icon"
    @update:model-value="$emit('update:model-value', $event)"
  >
    <v-menu
      activator="parent"
      :location="location"
      :close-on-content-click="closeOnContentClick"
    >
      <v-date-picker
        :elevation="elevation"
        @update:model-value="
                  (value: string) => {
                      $emit('update:model-value', value);
                  }
              "
      ></v-date-picker>
    </v-menu>
  </v-text-field>
</template>

<script lang="ts">
import { defineComponent, type PropType } from "vue";
export default defineComponent({
  name: "DateInput",
  props: {
    icon: {
      type: String,
      default: "mdi-calendar-today",
    },
    location: {
      type: String as PropType<"top" | "bottom">,
      default: "bottom",
    },
    elevation: {
      type: String,
      default: "6",
    },
    closeOnContentClick: {
      type: Boolean,
      default: false,
    },
  },
  emits: ["update:model-value"],
  data() {
    return {
      modelValue: "",
    };
  },
});
</script>
