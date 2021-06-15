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
  name: "Cinema",
};
</script>

<style lang="scss" scoped>
@import "@/scss/mixin";
.cinema {
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
  justify-content: flex-end;
  box-sizing: border-box;
  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
  @include for-phone {
    display: flex;
    flex-direction: column;
  }
}
.cinema-text {
  max-width: 503px;
  width: 100%;
  margin-right: 100px;
  box-sizing: border-box;
  text-align: start;

  @include for-tablet-landscape {
    margin-right: 0;
  }
  @include for-tablet-landscape {
    max-width: 400px;
    margin: 0 auto;
  }
}
.cinema-title {
  font-family: "Museo Sans Cyrl", sans-serif;
  position: absolute;
  color: #fff;
  opacity: 0.05;
  font-size: 75px;
  line-height: 1px;
  letter-spacing: 9px;
  padding-bottom: 100px;

  @include for-tablet-landscape {
    font-size: 47px;
  }
  @include for-phone {
    font-size: 20px;
    padding-top: 20px;
  }
}
.cinema-text__subtitle {
  margin-top: 50px;

  @include for-tablet-landscape {
    margin-top: 20px;
  }
}
.cinema-subtitle {
  font-family: "Roboto", sans-serif;
  font-size: 38px;
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
.cinema-description {
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  font-family: "Museo Sans Cyrl", sans-serif;

  @include for-tablet-landscape {
    font-size: 12px;
  }
}
.cinema-block {
  max-width: 503px;
  width: 100%;
  height: 360px;

  box-sizing: border-box;
  @include for-tablet-landscape {
    max-width: 400px;
    width: 100%;
    height: 300px;
    margin: 0 auto;
  }
}
.cinema-photo {
  max-width: 500px;
  width: 100%;
  height: 350px;

  @include for-tablet-landscape {
    max-width: 400px;
    width: 100%;
    height: 300px;
    margin: 0 auto;
  }
}
</style>