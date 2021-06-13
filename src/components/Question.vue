<template>
  <section class="question">
    <div class="container">
      <div class="question-text">
        <h2 class="question-title">
          Have <span class="color-text">any quastion</span>?
        </h2>
        <p class="contuct-us">Contact us!</p>
        <div class="btn">
          <button class="write" value="111001" name="name" type="submit">
            Write
          </button>
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

<style scoped>
.question {
  margin: 0 auto;
  padding: 0;
  max-width: 1440px;
  width: 100%;
  background-color: #171c1f;
  padding-top: 130px;
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
  font-size: 40px;
  line-height: 54px;
  color: #fff;
}
.color-text {
  color: #fdc400;
}
.contuct-us {
  font-size: 16px;
  line-height: 28px;
  color: #fff;
}
.btn {
  margin-top: 30px;
}
.write {
  max-width: 160px;
  width: 100%;
  border: 1px solid #fdc400;
  border-radius: 5px;
  padding: 10px 35px;
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  background-color: #161b1e;
}
.write:hover {
  background-color: #fdc400;
}
.question-photo {
  max-width: 641px;
  width: 100%;
  height: 479px;
  box-sizing: border-box;
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
  z-index: 50px;
}
</style>