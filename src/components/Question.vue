<template>
  <section class="question">
    <div class="container">
      <div class="question-text">
        <h2 class="question-title">
          Have <span class="color-text">any quastion</span>?
        </h2>
        <p class="contuct-us">Contact us!</p>
        <div class="btn">
          <a class="write" href="#1"> Write </a>
        </div>
      </div>
      <div class="question-blok__photo">
        <img src="/img/question.png" alt="" class="question-photo" />
      </div>
    </div>
    <div class="test">
      <div class="triangle-bottom-right"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Question",
};
</script>

<style lang="scss" scoped>
@import "@/scss/mixin";
.question {
  margin: 0 auto;
  padding: 0;
  max-width: 1440px;
  width: 100%;
  background-color: #171c1f;
  padding-top: 130px;

  @include for-tablet-landscape {
    padding-top: 90px;
  }
}
.container {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
}
.question-text {
  max-width: 390px;
  width: 100%;
  margin-right: 70px;
  box-sizing: border-box;
  text-align: start;
}
.question-title {
  font-family: "Roboto", sans-serif;
  font-size: 40px;
  line-height: 54px;
  color: #fff;

  @include for-tablet-landscape {
    font-size: 30px;
  }
  @include for-phone {
    font-size: 25px;
  }
}
.color-text {
  color: #fdc400;
}
.contuct-us {
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  font-family: "Roboto", sans-serif;

  @include for-tablet-landscape {
    font-size: 16px;
  }
  @include for-phone {
    font-size: 14px;
  }
}
.btn {
  margin-top: 30px;
}
.write {
  max-width: 160px;
  width: 100%;
  border: 1px solid #fdc400;
  border-radius: 5px;
  padding: 15px 60px;
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  background-color: #161b1e;
  text-decoration: none;
  font-family: "Roboto", sans-serif;
}
.write:hover {
  background-color: #fdc400;
}
.question-photo {
  max-width: 641px;
  width: 100%;
  height: 479px;
  box-sizing: border-box;

  @include for-tablet-landscape {
    max-width: 500px;
    height: 400px;
  }
}
.test {
  margin-top: -180px;
}
.triangle-bottom-right {
  position: relative;
  margin: 0 auto;
  max-width: 0;
  height: 0;
  border-bottom: 100px solid #fff;
  border-left: 1440px solid transparent;

  @include for-desktop {
    border-left: 954px solid transparent;
  }
}
</style>