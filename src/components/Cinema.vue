<template>
  <section class="cinema">
    <div class="container">
      <div class="cinema-text">
        <h2 class="cinema-title">CINEMA</h2>
        <div class="cinema-text__subtitle">
          <h2 class="cinema-subtitle">
            Cinema <span class="color-text">Glass</span>
          </h2>
        </div>
        <p class="cinema-description">
          Backed by our heritage of award winning lenses, we brought our
          cinematic glass to drones. Combined with our proprietary coatings,
          these filters deliver the smoothest, crispiest, color neutral image
          imaginable.
        </p>
      </div>
      <div class="cinema-block">
        <img class="cinema-photo" src="/img/cinema.png" alt="" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
    name:"Cinema",
};
</script>

<style scoped>
.cinema {
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
  justify-content: flex-end;
  box-sizing: border-box;
  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
}
.cinema-text {
  max-width: 503px;
  width: 100%;
  margin-right: 100px;
  box-sizing: border-box;
  text-align: start;
}
.cinema-title {
  position: absolute;
  color: #fff;
  opacity: 0.05;
  font-size: 75px;
  line-height: 1px;
  letter-spacing: 9px;
  padding-bottom: 100px;
}
.cinema-text__subtitle {
  margin-top: 50px;
}
.cinema-subtitle {
  font-size: 38px;
  line-height: 54px;
  color: #fff;
}
.color-text {
  color: #fdc400;
}
.cinema-description {
  font-size: 16px;
  line-height: 28px;
  color: #fff;
}
.cinema-block {
  max-width: 503px;
  width: 100%;
  height: 360px;

  box-sizing: border-box;
}
</style>