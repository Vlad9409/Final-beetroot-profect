<template>
  <section class="whowe">
    <div class="container">
      <div class="whowe-text">
        <h2 class="whowe-title">Who we are?</h2>

        <div class="whowe-text__subtitle">
          <p class="whowe-subtitle">
            Ready for whatever you can throw at them with advanced hydrophobic
            coatings, scratch resistant glass, and shatterproof construction.
            From Brooklyn to Iceland, these filters are prepared for takeoff
            wherever you feel like flying.
          </p>

          <div class="icon-more">
            <h3 class="whowe-more">Learn more</h3>
            <a href="#header" class="more">
              <img class="more" src="/img/more.svg" alt="" />
            </a>
          </div>
        </div>
      </div>
      <div class="whowe-blok">
        <img src="/img/Whoweare.png" alt="" class="whore-photo" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Whoweare",
};
</script>

<style lang="scss" scoped>
@import "@/scss/mixin";
.icon-more {
  display: flex;
  flex-direction: row;
  align-items: center;
}
.more {
  margin-left: 20px;

  @include for-tablet-landscape {
    width: 30px;
  }
}
.whowe {
  margin: 0 auto;
  padding: 0;
  max-width: 1440px;
  width: 100%;
  background-color: #171c1f;
}
.container {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
  @include for-phone {
    display: flex;
    flex-direction: column;
  }
}
.whowe-text {
  max-width: 365px;
  width: 100%;
  margin-right: 100px;
  box-sizing: border-box;
  text-align: start;

  @include for-tablet-landscape {
    width: 365px;
    margin-right: 100px;
    margin-left: 30px;
  }
  @include for-tablet-landscape {
    max-width: 500px;
    margin: 0 auto;
  }
}
.whowe-title {
  font-family: "Roboto", sans-serif;
  font-size: 40px;
  line-height: 54px;
  color: #fff;
  letter-spacing: 0.02em;
  padding-top: 40px;

  @include for-tablet-landscape {
    font-size: 30px;
  }
  @include for-phone {
    font-size: 25px;
  }
}
.whowe-subtitle {
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  font-family: "Museo Sans Cyrl", sans-serif;

  @include for-tablet-landscape {
    font-size: 12px;
  }
}

.whowe-more {
  font-size: 16px;
  line-height: 28px;
  display: flex;
  align-items: center;
  color: #fff;

  @include for-tablet-landscape {
    font-size: 12px;
  }
}
.whowe-blok {
  max-width: 737px;
  height: 399;
  box-sizing: border-box;
}
.whore-photo {
  max-width: 737px;
  width: 100%;
  height: 399;
  @include for-tablet-landscape {
    font-size: 12px;
  }
}
</style>