<template>
  <section id="bannerType" class="banner__wrap" :class="attr">
    <h2 class="blind">배너 영역</h2>
    <div class="banner__inner" :class="layout">
      <h3 class="title">#내_손으로_만들어_가는_루트</h3>
      <p class="desc">
        다양하고 다채로운 도시의 모습은 이곳을 참조하세요!<br />
        <a href="" title="유튜브 페이지로 이동"
          >https://www.youtube.com/channel/UCqVDpXKLmKeBU_yyt_QkItQ/</a
        >
      </p>
      <span class="small">도시 속 모습_01</span>
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
.banner__inner {
  background-image: url(../../assets/img/BANNER-TYPE01.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  text-align: center;
  padding: 120px 0;
  color: #fff;
}
.banner__inner .title {
  font-size: 50px;
  line-height: 1;
  font-weight: bold;
  padding-bottom: 20px;
  /* margin-bottom: 20px; */
}
.banner__inner .desc {
  font-size: 24px;
  line-height: 1.5;
  font-weight: 300;
  margin-bottom: 40px;
}
.banner__inner .desc a {
  color: #fff;
  display: inline-block;
  background: #00000021;
  backdrop-filter: blur(15px);
  border-radius: 5px;
  padding: 3px 10px;
  border: 1px solid #ffffff29;
  margin-top: 40px;
}
.banner__inner .desc a:hover {
  text-decoration: underline;
}
.banner__inner .small {
  font-size: 16px;
  /* text-decoration: underline; */
}

@media (max-width: 600px) {
  .banner__inner {
    padding: 120px 20px;
    box-sizing: border-box;
  }
  .banner__inner .desc a {
    text-overflow: ellipsis;
    overflow-y: clip;
    width: 60%;
  }
}
</style>
