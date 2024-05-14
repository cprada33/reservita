<template>
  <slot :checkbox="checkbox" :toggleCheckbox="toggleCheckbox"></slot>
</template>

<script setup>
import { ref, reactive } from 'vue';
import { db } from '../../Firebase/firebase.config';
import { getDocs, collection } from 'firebase/firestore';

const data = reactive({
  setup: null,
  punchline: null,
});

const fetching = ref(false);

const fetchReservas = async () => {
  fetching.value = true;
  const fetch = await getDocs(collection(db, 'reservas'));
  const reservas = await fetch.docs.map((doc) => ({
    id: doc.id,
    ...doc.data(),
  }));
  console.log(reservas);

  data.setup = reservas.setup;
  data.punchline = reservas.punchline;
  fetching.value = false;
};

fetchReservas();
</script>
