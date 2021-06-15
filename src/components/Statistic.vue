<template>
  <section class="statistic">
    <div class="container">
      <div class="statistic-title">
        <h2 class="statistic-title__text">
          Our <span class="color-text">statistics</span>
        </h2>
      </div>
      <div @scroll="handleScroll" class="statistik-circle">
        <div class="circle-big1">
          <div class="text1">1205</div>
          <svg>
            <circle class="bg1" cx="57" cy="57" r="52"></circle>
            <circle class="progress1" cx="57" cy="57" r="52"></circle>
          </svg>
        </div>
        <div class="circle-big2">
          <div class="text2">748</div>
          <svg>
            <circle class="bg2" cx="57" cy="57" r="52"></circle>
            <circle class="progress2" cx="57" cy="57" r="52"></circle>
          </svg>
        </div>
        <div class="circle-big3">
          <div class="text3">15</div>
          <svg>
            <circle class="bg3" cx="57" cy="57" r="52"></circle>
            <circle class="progress3" cx="57" cy="57" r="52"></circle>
          </svg>
        </div>
      </div>
      <div class="circle-text">
        <div class="circle-text1">
          <h3 class="circle-text__title">Sets were delivered</h3>
          <hr />
        </div>
        <div class="circle-text2">
          <h3 class="circle-text__title">People love us</h3>
          <hr />
        </div>
        <div class="circle-text3">
          <h3 class="circle-text__title">Sets we had to return</h3>
          <hr />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Statistic",
};
// data() {
// let last_known_scroll_position = 0;
// let ticking = false;

// function doSomething(scroll_pos) {
//   // Делаем что-нибудь с позицией скролла
// }

// window.addEventListener('scroll', function(e) {
//   last_known_scroll_position = window.scrollY;

//   if (!ticking) {
//     window.requestAnimationFrame(function() {
//       doSomething(last_known_scroll_position);
//       ticking = false;
//     });

//     ticking = true;
//   }
// });
// }
</script>

<style lang="scss" scoped>
@import "@/scss/mixin";
h2 {
  margin: 0;
  padding: 0;
}
.statistic {
  margin: 0 auto;
  padding: 130px 0 0 0;
  max-width: 1440px;
  width: 100%;
  background: #171c1f;

  @include for-tablet-landscape {
    padding: 90px 0 0 0;
  }
  @include for-tablet-landscape {
    display: flex;
    flex-direction: column;
    padding: 40px 0 0 0;
    margin: 0 auto;
  }
}
.container {
  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
}
.statistic-title__text {
  font-family: "Roboto", sans-serif;
  font-size: 40px;
  line-height: 54px;
  color: #fff;

  @include for-tablet-landscape {
    font-size: 30px;
  }
}
.color-text {
  color: #fdc400;
}

.statistik-circle {
  display: flex;
  flex-direction: row;
  justify-content: center;
  @include for-phone {
    display: flex;

    max-width: 400px;
    padding: 40px 0 0 0;
    margin: 0 auto;
  }
}

.circle-big1 {
  position: relative;
  width: 114px;
  height: 114px;
  margin: 30px 72px 25px 72px;
  @include for-phone {
    margin: 30px 32px 25px 32px;
  }
}

.circle-big1 svg {
  width: 114px;
  height: 114px;
}

.circle-big1 .bg1 {
  fill: none;
  stroke-width: 5px;
  stroke: #343035;
}

.circle-big1 .progress1 {
  fill: none;
  stroke-width: 5px;
  stroke: #fdc400;
  stroke-linecap: round;
  stroke-dasharray: 325;
  stroke-dashoffset: 60;
  transform: rotate(336deg);
  transform-origin: 50% 50%;
  animation: big 1.5s ease-in-out both;
}
@keyframes big {
  from {
    stroke-dashoffset: 326.56;
  }
  to {
    stroke-dashoffset: 60;
  }
}
.circle-big1 .text1 {
  position: absolute;
  width: 100%;
  top: 45px;
  font-size: 30px;
  text-align: center;
  font-weight: 400;
  line-height: 22px;
}

.circle-big1 .text1 {
  text-align: center;
  font-size: 24px;
  color: #fff;
  font-family: "Roboto", sans-serif;
}

.circle-big2 {
  position: relative;
  width: 114px;
  height: 114px;
  margin: 30px 72px 25px 72px;
  @include for-phone {
    margin: 30px 32px 25px 32px;
  }
}

.circle-big2 svg {
  width: 114px;
  height: 114px;
}

.circle-big2 .bg2 {
  fill: none;
  stroke-width: 5px;
  stroke: #343035;
}

.circle-big2 .progress2 {
  fill: none;
  stroke-width: 5px;
  stroke: #fdc400;
  stroke-linecap: round;
  stroke-dasharray: 325;
  stroke-dashoffset: 85;
  transform: rotate(365deg);
  transform-origin: 50% 50%;
  animation: big2 1.5s ease-in-out;
}
@keyframes big2 {
  from {
    stroke-dashoffset: 325;
  }
  to {
    stroke-dashoffset: 85;
  }
}

.circle-big2 .text2 {
  position: absolute;
  width: 100%;
  top: 45px;
  font-size: 30px;
  text-align: center;
  font-weight: 400;
  line-height: 22px;
}

.circle-big2 .text2 {
  text-align: center;
  font-size: 24px;
  color: #fff;
}

.circle-big3 {
  position: relative;
  width: 114px;
  height: 114px;
  margin: 30px 72px 25px 72px;
  @include for-phone {
    margin: 30px 32px 25px 32px;
  }
}

.circle-big3 svg {
  width: 114px;
  height: 114px;
}

.circle-big3 .bg3 {
  fill: none;
  stroke-width: 5px;
  stroke: #343035;
}

.circle-big3 .progress3 {
  fill: none;
  stroke-width: 5px;
  stroke: #fdc400;
  stroke-linecap: round;
  stroke-dasharray: 325;
  stroke-dashoffset: 275;
  transform: rotate(90deg);
  transform-origin: 50% 50%;
  animation: big3 1.5s ease-in-out;
}
@keyframes big3 {
  from {
    stroke-dashoffset: 325;
  }
  to {
    stroke-dashoffset: 275;
  }
}

.circle-big3 .text3 {
  position: absolute;
  width: 100%;
  top: 45px;
  font-size: 30px;
  text-align: center;
  font-weight: 400;
  line-height: 22px;
}

.circle-big3 .text3 {
  text-align: center;
  font-size: 24px;
  color: #fff;
}

.circle-text {
  margin: 0 auto;
  display: flex;
  max-width: 710px;
  width: 100%;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  @include for-phone {
    justify-content: space-around;
  }
}

.circle-text__title {
  font-size: 18px;
  line-height: 26px;
  color: #fff;

  @include for-tablet-landscape {
    font-size: 14px;
  }
}

.circle-text1 {
  margin-right: 120px;

  @include for-tablet-landscape {
    margin-right: 50px;
    padding-left: 30px;
  }
}
.circle-text3 {
  margin-left: 110px;

  @include for-tablet-landscape {
    margin-left: 50px;
    margin-right: 20px;
  }
}

hr {
  max-width: 40px;
  width: 100%;
  border: none;
  background-color: #fdc400;
  color: #fdc400;
  height: 1px;
}
</style>