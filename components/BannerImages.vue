<template>
  <div :class="styling.bannerClass">
    <div
      v-for="link in images"
      :class="styling.divClass"
      :style="styling.divStyle"
    >
      <img
        :src="link"
        alt="imagen"
        :style="styling.imgStyle"
        :class="styling.imgClass"
      />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    styling: Object,
    images: Object,
  },
};
</script>
