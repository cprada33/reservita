<template>
  <HomeBanner />
  <BannerImages :styling="styling" :images="images" />
  <BannerImages :styling="stylingCabanas" :images="imagesCabanas" />
</template>

<script>
export default {
  data() {
    return {
      styling: {
        bannerClass:
          'd-flex flex-wrap justify-space-between align-content-start flex-grow-0',
        divStyle: 'max-height: 30%',
        divClass: 'v-col-3',
        imgStyle: 'height: 100%; width: 100%; object-fit: cover',
        imgClass: 'rounded-xl',
      },
      stylingCabanas: {
        bannerClass:
          'd-flex flex-wrap justify-space-between align-content-start',
        divStyle: 'max-height: 70%',
        divClass: 'v-col-3 text-center',
        imgStyle: 'height: 100%; width: 90%; object-fit: cover',
      },
      images: [
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
      ],
      imagesCabanas: [
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fkashi.jpg?alt=media&token=f2381d8f-ae0e-4f92-a826-754a98a8a220',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fkashi.jpg?alt=media&token=f2381d8f-ae0e-4f92-a826-754a98a8a220',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fkashi.jpg?alt=media&token=f2381d8f-ae0e-4f92-a826-754a98a8a220',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fkashi.jpg?alt=media&token=f2381d8f-ae0e-4f92-a826-754a98a8a220',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fkashi.jpg?alt=media&token=f2381d8f-ae0e-4f92-a826-754a98a8a220',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fkashi.jpg?alt=media&token=f2381d8f-ae0e-4f92-a826-754a98a8a220',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fkashi.jpg?alt=media&token=f2381d8f-ae0e-4f92-a826-754a98a8a220',
        'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fkashi.jpg?alt=media&token=f2381d8f-ae0e-4f92-a826-754a98a8a220',
      ],
    };
  },
};
</script>
