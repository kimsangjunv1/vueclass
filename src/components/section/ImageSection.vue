<template>
  <section id="imageType01" class="image__wrap" :class="attr">
    <h2>#내_여행_동반자</h2>
    <p>내 여행동안 내 외로움을 채워줄 소울 메이트는 어떠세요?</p>
    <div class="image__inner" :class="layout">
      <article class="image img1">
        <h3 class="image__title">불독은 어떠세요?</h3>
        <p class="image__desc">
          불독은 혼종이라고 하는데, 사람들에게 인기많은 이유는<br />
          생김새를 떠나서 강아지를 키운다는 그 사실이 좋은겁니다.
        </p>
        <a class="image__btn yellow loading" href="/" title="자세히 보기"
          >자세히 보기</a
        >
      </article>
      <article class="image img2">
        <h3 class="image__title">웰시코기는 어떠세요?</h3>
        <p class="image__desc">
          웰시코기는 다리가 참 짧죠? 그래서 키우는 사람들도 많은 편이고<br />
          총총 걸어다니는 모습을 보고있자니 너무 귀엽답니다!
        </p>
        <a class="image__btn loading" href="/" title="자세히 보기"
          >자세히 보기</a
        >
      </article>
    </div>
  </section>
</template>
<script>
export default {
  props: {
    attr: String,
    layout: String,
  },
};
</script>

<style>
.image__inner {
  display: flex;
  justify-content: space-between;
}
.image {
  width: 49%;
  height: 370px;
  color: #fff;
  padding: 200px 30px 30px 30px;
  box-sizing: border-box;
  border-radius: 5px;
}
.image.img1 {
  background: url(../../assets/img/bg01_01.jpg) no-repeat center;
  background-size: cover;
}
.image.img2 {
  background: url(../../assets/img/bg01_02.jpg) no-repeat center;
  background-size: cover;
}
.image__title {
  font-size: 32px;
  margin-bottom: 10px;
}
.image__desc {
  font-size: 16px;
  font-weight: 300;
  margin-bottom: 10px;
  line-height: 1.5;
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}
.image__btn {
  font-size: 16px;
  color: #fff;
  background-color: #b45a30;
  padding: 10px 20px;
  display: inline-block;
  border-radius: 5px;
}
.image__btn:hover .img1 {
  scale: 1.2;
  transition: 0.25s;
}
.image__btn.yellow {
  background-color: #b59140;
}

@media (max-width: 1215px) {
  .container {
    width: 100%;
  }
  .image {
    width: 100%;
  }
  .image:nth-child(1) {
    margin-bottom: 20px;
  }
  .image__inner {
    flex-wrap: wrap;
    padding: 10px;
  }
  .image__title {
    font-size: 24px;
  }
}

@media (max-width: 1220px) {
  .slider__inner {
    margin-top: 0 !important;
  }
}

@media (max-width: 750px) {
  .section > h2 {
    font-size: 30px;
  }
  .section > p {
    font-size: 16px;
  }
}
</style>
