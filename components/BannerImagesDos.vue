<template>
  <div class="d-flex flex-wrap justify-space-between align-content-start">
    <div v-for="link in images" class="v-col-3" style="max-height: 30%">
      <img
        :src="link"
        alt="imagen"
        style="height: 100%; width: 100%; object-fit: cover"
        class="rounded-xl"
      />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    bannerClass: String,
    bannerStyle: String,
    imgStyle: String,
    imgClass: String,
    divClass: String,
    images: String,
  },
};
let images = [
  'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
  'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
  'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
  'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
  'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
  'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
  'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
  'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
];
</script>
