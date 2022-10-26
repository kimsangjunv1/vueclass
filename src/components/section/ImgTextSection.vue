<template>
  <section id="imgTextType" class="imgText__wrap" :class="attr">
    <h2 class="blind">유용한 사이트 살펴보기 🎮</h2>
    <div class="imgText__inner container" :class="layout">
      <div class="imgText__txt">
        <span>여행 속 내 비즈니스</span>
        <h3>#일은_절대_놓을_수_없지</h3>
        <p>우리 다 같이 도시 라이프를 다채로운 방식으로 함께 즐겨보아요!</p>
        <ul>
          <li><a href="/">오늘의 티</a></li>
          <li><a href="/">오늘의 공원</a></li>
          <li><a href="/">오늘의 장소</a></li>
          <li><a href="/">오늘의 가게</a></li>
          <li><a href="/">오늘의 춤</a></li>
          <li><a href="/">오늘의 회사 출근 음악</a></li>
        </ul>
      </div>
      <div class="imgText__img img1">
        <a href="/">비즈니스</a>
      </div>
      <div class="imgText__img img2">
        <a href="/" class="blue">작업할때</a>
      </div>
    </div>
  </section>
</template>

<style>
/* imgTextType */
.imgText__inner {
  display: flex;
  justify-content: space-between;
}

.imgText__inner > div {
  width: 32%;
  height: 500px;
}
.imgText__txt {
}
.imgText__txt span {
  font-size: 16px;
  color: #666;
  text-decoration: underline;
  text-underline-position: under;
  margin-bottom: 20px;
}
.imgText__txt h3 {
  font-size: 50px;
  font-weight: bold;
  word-break: keep-all;
  line-height: 1.4;
  margin-bottom: 20px;
  margin-top: 20px;
}
.imgText__txt p {
  font-size: 18px;
  font-weight: 300;
  line-height: 1.5;
  color: #666;
  margin-bottom: 10px;
}
.imgText__txt ul {
  font-size: 18px;
  font-weight: 300;
  line-height: 1.6;
}
.imgText__txt ul li {
  position: relative;
  padding-left: 20px;
}

.imgText__txt ul li a {
  color: #666;
}

.imgText__txt ul li::before {
  content: "";
  width: 5px;
  height: 5px;
  border-radius: 50%;
  position: absolute;
  left: 5px;
  top: 9px;
  background: #666;
}

.imgText__img {
  border-radius: 10px;
  position: relative;
}

.imgText__img a {
  position: absolute;
  left: 30px;
  bottom: 30px;
  background-color: #7c2b39;
  color: #fff;
  font-size: 18px;
  padding: 10px 30px;
  border-radius: 30px;
  display: inline-block;
}
.imgText__img a.blue {
  background-color: #2b387c;
}
.imgText__img.img1 {
  background: url(../../assets/img/imgText_bg01.jpg) no-repeat center / cover;
}
.imgText__img.img2 {
  background: url(../../assets/img/imgText_bg02.jpg) no-repeat center / cover;
}

@media (max-width: 600px) {
  .imgText__inner {
    display: block;
    padding: 20px;
    box-sizing: border-box;
  }
  .imgText__img {
    margin-bottom: 20px;
  }
  .imgText__inner > div {
    width: 100%;
    /* height: 385px; */
  }
  .section:nth-child(3) {
    padding: 20px 0;
  }
}
</style>
