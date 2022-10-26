<template>
  <section id="sliderType" class="slider__wrap" :class="attr">
    <h2 class="blind">슬라이드 영역</h2>
    <div class="slider__inner" :class="layout">
      <swiper
        :spaceBetween="30"
        :centeredSlides="true"
        :autoplay="{
          delay: 2500,
          disableOnInteraction: false,
        }"
        :pagination="{
          clickable: true,
        }"
        :navigation="true"
        :modules="modules"
        class="mySwiper"
      >
        <swiper-slide>
          <div class="desc">
            <span>어디로 가볼까?</span>
            <h3>#새하얀_눈.</h3>
            <p>눈 덮힌 마을 속 고히 잠들어 있는 새싹들</p>
            <div class="btn">
              <a class="loading" href="/"> 자세히 보기 </a>
              <a href="/" class="black loading"> 사이트 보기 </a>
            </div>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="desc">
            <span>어디로 가볼까?</span>
            <h3>#새하얀_눈.</h3>
            <p>눈 덮힌 마을 속 고히 잠들어 있는 새싹들</p>
            <div class="btn">
              <a class="loading" href="/"> 자세히 보기 </a>
              <a href="/" class="black loading"> 사이트 보기 </a>
            </div>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="desc">
            <span>어디로 가볼까?</span>
            <h3>#새하얀_눈.</h3>
            <p>눈 덮힌 마을 속 고히 잠들어 있는 새싹들</p>
            <div class="btn">
              <a class="loading" href="/"> 자세히 보기 </a>
              <a href="/" class="black loading"> 사이트 보기 </a>
            </div>
          </div>
        </swiper-slide>
      </swiper>
    </div>
  </section>
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

// import "../style.css";

// import required modules
import { Autoplay, Pagination, Navigation } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
    };
  },
};
</script>

<style>
.slider__inner {
  margin-top: 70px;
  position: relative;
  overflow: hidden;
}

.slider {
  position: relative;
}

.slider:not(:hover) .slider__img {
  transition: 0.25s;
}

.slider:hover .slider__img {
  /* background: #000; */
  transform: scale(1.1);
  transition: 0.25s;
}

.slider__img {
  /* background: url(../../assets/img/slider_bg01.jpg) no-repeat center / cover; */
}

.slider__img.show.one {
  display: block;
}

.one {
  background: url(../../assets/img/slider_bg01.jpg) no-repeat center / cover;
  display: none;
  z-index: 0;
  position: relative;
}
.three::before,
.two::before,
.one::before {
  content: "";
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.387);
  position: absolute;
  z-index: -1;
}
.two {
  background: url(../../assets/img/slider_bg02.jpg) no-repeat center / cover;
  display: none;
  z-index: 0;

  position: relative;
}
.three {
  background: url(../../assets/img/slider_bg03.jpg) no-repeat center / cover;
  display: none;
  z-index: 0;

  position: relative;
}

.show {
  display: block;
}

.slider__img .desc {
  /* width: 1160px; */
  /* margin: 0 auto; */
  padding: 100px;
  text-align: center;
}
.slider__img .desc span {
  font-size: 16px;
  background-color: #ffffff17;
  padding: 7px 10px;
  text-transform: uppercase;
  margin-bottom: 10px;
  display: inline-block;
  backdrop-filter: blur(15px);
  -webkit-backdrop-filter: blur(15px);
  border-top: 1px solid #fff;
  border-bottom: 1px solid #fff;
  color: #fff;
}
.slider__img .desc h3 {
  font-size: 90px;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-transform: uppercase;
  margin-bottom: 16px;
  margin-left: -8px;
  margin-top: 20px;
}
.slider__img .desc p {
  font-size: 20px;
  font-weight: 300;
  color: #fff;
  line-height: 1.35;
  margin-bottom: 80px;
}

.slider__img .desc .btn {
}
.slider__img .desc .btn a {
  font-size: 16px;
  background-color: rgba(255, 255, 255, 0.537);
  backdrop-filter: blur(15px);
  -webkit-backdrop-filter: blur(15px);
  padding: 11px 30px;
  display: inline-block;
  border-radius: 5px;
  border: 1px solid rgba(255, 255, 255, 0.48);
}
.slider__img .desc .btn a.black {
  background: rgba(0, 0, 0, 0.457);
  color: #fff;
}
.slider__arrow {
  z-index: 5;
}
.slider__dot {
  z-index: 5;
}

.slider__arrow a {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  width: 30px;
  height: 56px;
  background-image: url(../../assets/img/slider_icon.svg);
}
.slider__arrow a.left {
  left: 20px;
}
.slider__arrow a.right {
  right: 20px;
  background-position: -50px 0;
}
.slider__dot {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  bottom: 25px;
}

.slider__dot a {
  display: inline-block;
  width: 16px;
  height: 16px;
  background-image: url(../../assets/img/slider_icon.svg);
  background-position: -20px -70px;
}

.slider__dot a.active {
  background-position: 0px -70px;
}

.slider__dot a.play {
  background-position: -40px -70px;
}

.slider__dot a.stop {
  background-position: -60px -70px;
}

.slider {
  position: relative;
}
.swiper-button {
  position: absolute;
  left: 50%;
  bottom: 24px;
  z-index: 1000;
  margin-left: 40px;
}
.swiper-button-stop {
  background-image: url(../../assets/img/slider_icon.svg);
  background-position: -40px -70px;
  width: 16px;
  height: 16px;
  cursor: pointer;
}
.swiper-button-play {
  background-image: url(../../assets/img/slider_icon.svg);
  background-position: -60px -70px;
  width: 16px;
  height: 16px;
  cursor: pointer;
  display: none;
}

.swiper-slide {
  background: url(../../assets/img/slider_bg01.jpg) no-repeat center / cover;
  height: 500px;
}

.swiper-slide:nth-child(2) {
  background: url(../../assets/img/slider_bg02.jpg) no-repeat center / cover;
}

.swiper-slide:nth-child(3) {
  background: url(../../assets/img/slider_bg03.jpg) no-repeat center / cover;
}

.swiper-slide .desc {
  /* width: 1160px; */
  /* margin: 0 auto; */
  padding: 100px;
  text-align: center;
}
.swiper-slide .desc span {
  font-size: 16px;
  background-color: #ffffff17;
  padding: 7px 10px;
  text-transform: uppercase;
  margin-bottom: 10px;
  display: inline-block;
  backdrop-filter: blur(15px);
  -webkit-backdrop-filter: blur(15px);
  border-top: 1px solid #fff;
  border-bottom: 1px solid #fff;
  color: #fff;
}
.swiper-slide .desc h3 {
  font-size: 90px;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-transform: uppercase;
  margin-bottom: 16px;
  margin-left: -8px;
  margin-top: 20px;
}
.swiper-slide .desc p {
  font-size: 20px;
  font-weight: 300;
  color: #fff;
  line-height: 1.35;
  margin-bottom: 20px;
}

.swiper-slide .desc .btn {
}
.swiper-slide .desc .btn a {
  font-size: 16px;
  background-color: rgba(255, 255, 255, 0.537);
  backdrop-filter: blur(15px);
  -webkit-backdrop-filter: blur(15px);
  padding: 11px 30px;
  display: inline-block;
  border-radius: 5px;
  border: 1px solid rgba(255, 255, 255, 0.48);
}
.swiper-slide .desc .btn a.black {
  background: rgba(0, 0, 0, 0.457);
  color: #fff;
}

.swiper-pagination-bullet {
  /* display: inline-block; */
  width: 16px;
  height: 16px;
  background-image: url(../../assets/img/slider_icon.svg);
  background-position: -20px -70px;
  opacity: 1;
  background-color: #000 !important;
}
.swiper-pagination-bullet-active {
  background-position: 0px 70px !important;
}

/* media */
@media (max-width: 920px) {
  .slider__img .desc h3 {
    font-size: 50px;
  }
}
@media (max-width: 960px) {
  .swiper-slide .desc p {
    margin-bottom: 60px;
    font-size: 16px;
  }
  .swiper-slide {
    text-align: center;
  }
  .swiper-slide .desc h3 {
    font-size: 60px;
  }
  .swiper-slide .desc {
    width: 100%;
    padding: 0;
    text-align: center;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}
</style>
