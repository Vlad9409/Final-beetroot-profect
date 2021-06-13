<template>
  <section class="shatter">
    <div class="container">
      <div class="block-shatter">
        <img class="photo-shatte" src="/img/Shatter.png" alt="" />
      </div>
      <div class="shatter-text">
        <div class="shatter-text__block">
          <h2 class="shatter-text__title">SHATTER</h2>
        </div>
        <div class="shatter-text__subtitle">
          <h2 class="cinema-subtitle">Shatterproof Construction</h2>
        </div>
        <div class="cinema-text__description">
          <p class="shatter-description">
            Ready for whatever you can throw at them with advanced hydrophobic
            coatings, scratch resistant glass, and shatterproof construction.
            From Brooklyn to Iceland, these filters are prepared for takeoff
            wherever you feel like flying.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Shatter",
};
</script>

<style scoped>
.shatter {
  margin: 0 auto;
  padding: 0;
  padding-top: 160px;
  max-width: 1440px;
  width: 100%;
  background-color: #171c1f;
}
.container {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
}
.photo-shatte {
  max-width: 490px;
  width: 100%;
  height: 680px;
  margin-left: 3px;
}
.shatter-text {
  max-width: 550px;
  width: 100%;
  margin-left: 96px;
}
.shatter-text__title {
  position: absolute;
  color: #fff;
  opacity: 0.05;
  font-size: 75px;
  line-height: 1px;
  letter-spacing: 9px;
}
.cinema-subtitle {
  font-size: 40px;
  line-height: 54px;
  color: #fff;
}
.shatter-text__subtitle {
  padding-top: 30px;
  text-align: start;
}
.shatter-description {
  font-size: 14px;
  line-height: 28px;
  color: #fff;
  letter-spacing: 1px;
}
.cinema-text__description {
  max-width: 570px;
  width: 100%;
  text-align: start;
}
</style>