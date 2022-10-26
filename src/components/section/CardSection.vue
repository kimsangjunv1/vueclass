<template>
  <section id="cardType" class="card__wrap" :class="attr">
    <!--다중 클래스 선택-->
    <h2>#여행_중_게임은_못참지🎮</h2>
    <p>
      새롭고 혁신적인 PS5™ 컨트롤러로 완전히 몰입할 수 있는 게임 경험을
      즐겨보시기 바랍니다.
    </p>
    <div class="card__inner" :class="layout">
      <article class="card">
        <figure class="card__header">
          <!--img를 쓰기 위한 웹 표준 방법-->
          <img
            src="../../assets/img/card_bg01_01.jpg"
            alt="다양한 인터렉티브 반응"
          />
        </figure>
        <div class="card__body">
          <h3 class="tit">다양한 인터렉티브 반응</h3>
          <p class="desc">
            인게임 기어 및 환경과 상호작용하면서 활시위를 당길 때 점점
            팽팽해지는 느낌과 질주하는 자동차의 급브레이크를 밟는 느낌 등 액션과
            함께 어우러집니다.
          </p>
          <a class="btn loading" href="/">
            더 자세히 보기
            <span aria-hidden="true">
              <!--aria-hidden="true" 로 처리시 이 부분을 읽는것을 스킵한다.-->
              <svg
                width="65"
                height="8"
                viewBox="0 0 65 8"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M64.3536 4.35355C64.5488 4.15829 64.5488 3.84171 64.3536 3.64645L61.1716 0.464466C60.9763 0.269204 60.6597 0.269204 60.4645 0.464466C60.2692 0.659728 60.2692 0.976311 60.4645 1.17157L63.2929 4L60.4645 6.82843C60.2692 7.02369 60.2692 7.34027 60.4645 7.53553C60.6597 7.7308 60.9763 7.7308 61.1716 7.53553L64.3536 4.35355ZM0 4.5H64V3.5H0V4.5Z"
                  fill="black"
                />
              </svg>
            </span>
          </a>
        </div>
      </article>
      <article class="card">
        <figure>
          <!--img를 쓰기 위한 웹 표준 방법-->
          <img src="../../assets/img/card_bg01_02.jpg" alt="게임패드 지원" />
        </figure>
        <div class="card__body">
          <h3 class="tit">게임패드 지원</h3>
          <p class="desc">
            내장 마이크를 사용하거나 3.5mm 잭에 미니멀하고 아이코닉한 헤드셋을
            연결 전용 음소거 버튼을 사용하여 음성 캡처를 즉시 끌 수 있습니다.
          </p>
          <a class="btn loading" href="/">
            더 자세히 보기
            <span aria-hidden="true">
              <svg
                width="65"
                height="8"
                viewBox="0 0 65 8"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M64.3536 4.35355C64.5488 4.15829 64.5488 3.84171 64.3536 3.64645L61.1716 0.464466C60.9763 0.269204 60.6597 0.269204 60.4645 0.464466C60.2692 0.659728 60.2692 0.976311 60.4645 1.17157L63.2929 4L60.4645 6.82843C60.2692 7.02369 60.2692 7.34027 60.4645 7.53553C60.6597 7.7308 60.9763 7.7308 61.1716 7.53553L64.3536 4.35355ZM0 4.5H64V3.5H0V4.5Z"
                  fill="black"
                />
              </svg>
            </span>
          </a>
        </div>
      </article>
      <article class="card">
        <figure>
          <!--img를 쓰기 위한 웹 표준 방법-->
          <img
            src="../../assets/img/card_bg01_03.jpg"
            alt="진동을 통한 생생한 현장감"
          />
        </figure>
        <div class="card__body">
          <h3 class="tit">진동을 통한 생생한 현장감</h3>
          <p class="desc">
            기존의 진동 모터 대신 듀얼 액추에이터가 선사하는 물리적 반응형
            피드백을 경험해보세요, 게임 내 환경에서부터 실감 나는 역동적인
            진동이 손을 타고 전해집니다.
          </p>
          <a class="btn loading" href="/">
            더 자세히 보기
            <span aria-hidden="true">
              <svg
                width="65"
                height="8"
                viewBox="0 0 65 8"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M64.3536 4.35355C64.5488 4.15829 64.5488 3.84171 64.3536 3.64645L61.1716 0.464466C60.9763 0.269204 60.6597 0.269204 60.4645 0.464466C60.2692 0.659728 60.2692 0.976311 60.4645 1.17157L63.2929 4L60.4645 6.82843C60.2692 7.02369 60.2692 7.34027 60.4645 7.53553C60.6597 7.7308 60.9763 7.7308 61.1716 7.53553L64.3536 4.35355ZM0 4.5H64V3.5H0V4.5Z"
                  fill="black"
                />
              </svg>
            </span>
          </a>
        </div>
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
/* cardType */
.card__inner {
  display: flex;
  /* 생성한 요소들을 flex로 정렬합니다. */
  justify-content: space-between;
  /*창 크기에 맞게 좌우로 정렬합니다 */
  /*콘텐츠를 양쪽으로 정렬*/
}

.card {
  width: 32%;
  background-color: #f5f5f5;
}

.card__body {
  padding: 24px;
}

.card__body .tit {
  font-size: 24px;
  margin-bottom: 10px;

  /* 한줄 효과 */
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
  padding-right: 20px;
}

.card__body .desc {
  font-size: 18px;
  line-height: 1.4;
  color: #666;
  margin-bottom: 20px;
  font-weight: 300;

  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 4; /*줄 효과*/
  -webkit-box-orient: vertical;
}
.card:hover span {
  margin-left: 30px;
  transition: 0.4s;
}
.card:hover img {
  scale: 1.2;
  overflow: hidden;
  transition: 0.25s;
}
.card:not(:hover) span,
.card:not(:hover) img {
  transition: 0.25s;
}
figure {
  overflow: hidden;
}

@media (max-width: 600px) {
  .card__inner {
    display: block;
  }
  .card {
    width: 100%;
  }
  .card:nth-child(1),
  .card:nth-child(2) {
    margin-bottom: 20px;
  }
  .section:nth-child(4) {
    padding: 120px 20px;
    box-sizing: border-box;
  }
}
</style>
