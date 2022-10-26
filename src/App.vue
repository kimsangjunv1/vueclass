<!-- html -->
<template>
  <div>
    <HeaderLayout fonts="nexon" />
    <SliderSection attr="baegopa" layout="container" />
    <ImageSection attr="nexon section baegopa" layout="container" />
    <CardSection attr="nexon section baegopa" layout="container" />
    <ImgTextSection attr="nexon section gray baegopa" layout="container" />
    <BannerSection attr="nexon section baegopa" />
    <TextSection attr="nexon section baegopa" layout="container" />
    <FooterLayout attr="nexon section gray baegopa" />
  </div>
</template>

<!-- js -->
<script>
import HeaderLayout from "./components/layout/HeaderLayout.vue";
import FooterLayout from "./components/layout/FooterLayout.vue";
import SliderSection from "./components/section/SliderSection.vue";
import ImgTextSection from "./components/section/ImgTextSection.vue";
import ImageSection from "./components/section/ImageSection.vue";
import CardSection from "./components/section/CardSection.vue";
import TextSection from "./components/section/TextSection.vue";
import BannerSection from "./components/section/BannerSection.vue";

export default {
  name: "App",
  components: {
    HeaderLayout,
    FooterLayout,
    SliderSection,
    CardSection,
    ImgTextSection,
    ImageSection,
    TextSection,
    BannerSection,
  },
};
</script>
, CardSection
