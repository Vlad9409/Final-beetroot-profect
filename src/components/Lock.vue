<template>
  <section class="lock">
    <div class="container">
      <div class="block-lock">
        <img class="photo-lock" src="/img/lock.png" alt="" />
      </div>
      <div class="lock-text">
        <h2 class="lock-text__title">LOCK</h2>
        <div class="lock-text__subtitle">
          <h2 class="lock-subtitle">
            <span class="color-text">Lock</span> and
            <span class="color-text">balance</span> mounting system
          </h2>
        </div>
        <p class="lock-description">
          There is no standard for how to attach and balance a lens on a drone,
          so we made one. Introducing our Lock and Balance Mounting System. It’s
          a two part design with a lens on one side and a counterweight on the
          other. The two parts clamp together over the drone’s camera, creating
          a secure lock that doesn’t impede the gimbal.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Lock",
};
</script>

<style scoped>
.lock {
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

  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
}
.lock-text__title {
  position: absolute;
  color: #fff;
  opacity: 0.05;
  font-size: 75px;
  line-height: 1px;
  letter-spacing: 9px;
  padding-bottom: 100px;
}
.lock-text__subtitle {
  position: relative;
  padding-top: 20px;
  max-width: 574px;
}
.lock-text {
  max-width: 662px;
  width: 100%;
  text-align: start;
  box-sizing: border-box;
  margin-left: 98px;
}
.lock-description {
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  letter-spacing: 1px;
}
.lock-subtitle {
  font-size: 40px;
  line-height: 54px;
  color: #fff;
}
.photo-lock {
  max-width: 500px;
  width: 100%;
  height: 350px;
}
.color-text {
  color: #fdc400;
}
</style>
