<template>
  <footer id="footerType" class="footer__wrap" :class="attr">
    <h2 class="blind">푸터 영역</h2>
    <div class="footer__inner">
      <div class="footer__menu">
        <div>
          <h3>도움말</h3>
          <ul>
            <li><a href="/">사이트 사용법</a></li>
            <li><a href="/">도움말 찾기</a></li>
            <li><a href="/">사이트맵</a></li>
            <li><a href="/">각 메뉴 설명</a></li>
          </ul>
        </div>
        <div>
          <h3>행복상담</h3>
          <ul>
            <li><a href="/">고민거리</a></li>
            <li><a href="/">미래</a></li>
            <li><a href="/">과거</a></li>
          </ul>
        </div>
        <div>
          <h3>여행</h3>
          <ul>
            <li><a href="/">한국</a></li>
            <li><a href="/">중국</a></li>
            <li><a href="/">일본</a></li>
            <li><a href="/">싱가포르</a></li>
            <li><a href="/">말레이시아</a></li>
          </ul>
        </div>
        <div>
          <h3>팁</h3>
          <ul>
            <li><a href="/">여행가이드</a></li>
            <li><a href="/">위치</a></li>
            <li><a href="/">사진스팟</a></li>
          </ul>
        </div>
        <div>
          <h3>고객센터</h3>
          <ul>
            <li><a href="/">여행 상담</a></li>
            <li><a href="/">고민 상담</a></li>
            <li><a href="/">권고 상담</a></li>
            <li><a href="/">행복 상담</a></li>
          </ul>
        </div>
        <div>
          <h3>사업자등록</h3>
          <ul>
            <li><a href="/">1. 표준사항</a></li>
            <li><a href="/">2. 법사항</a></li>
            <li><a href="/">3. 규범사항</a></li>
            <li><a href="/">4. 참조사항</a></li>
            <li><a href="/">5. 준수사항</a></li>
            <li><a href="/">6. 권고사항</a></li>
          </ul>
        </div>
      </div>
      <div class="footer__right">
        2022 CODi. Portfolio is power<br />
        All rights reserved.
      </div>
    </div>
  </footer>
</template>

<style>
.footer__menu {
  display: flex;
}
.footer__menu > div {
  width: 16%;
  margin-bottom: 70px;
}

.footer__menu > div h3 {
  font-size: 18px;
  margin-bottom: 20px;
}

.footer__menu li a {
  font-size: 14px;
  color: #666;
  margin-bottom: 10px;
  display: block;
}

.footer__right {
  border-top: 1px solid #d9d9d9;
  text-align: center;
  padding-top: 40px;
  color: #666;
  line-height: 1.5;
}
@media (max-width: 900px) {
  .footer__menu {
    flex-wrap: wrap;
  }
}
</style>
