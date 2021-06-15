<template>
  <section class="deliver">
    <div class="container">
      <div class="deliver-text">
        <h2 class="deliver-title">HOW</h2>
        <div class="deliver-text__subtitle">
          <h2 class="deliver-subtitle">
            How do we <span class="color-text">deliver</span>?
          </h2>
        </div>
        <div class="icon-more">
          <h3 class="deliver-more">Learn more</h3>
          <a href="#header" class="more">
            <img class="more" src="/img/more.svg" alt="" />
          </a>
        </div>
      </div>
      <div class="description">
        <p class="description-title">
          Your order is important to us! We make every effort to deliver your
          order in a timely manner. Before you place your order, please read
          through the various delivery options and pick the method that best
          suits your needs. Questions? Send us a quick email to orders@bdel.com
          and we'll get you an answer promptly.
        </p>
        <p class="description-title">
          Most orders are shipped the next business day after we receive your
          order.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Deliver",
};
</script>

<style lang="scss" scoped>
@import "@/scss/mixin";
.deliver {
  margin: 0 auto;
  padding: 0;
  max-width: 1440px;
  width: 100%;
  background-color: #171c1f;
  padding-top: 70px;
}
.container {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
}
.deliver-text {
  max-width: 370px;
  width: 100%;
  margin-right: 100px;
  box-sizing: border-box;
  text-align: start;
}
.deliver-title {
  position: absolute;
  color: #fff;
  opacity: 0.05;
  font-size: 100px;
  line-height: 1px;
  letter-spacing: 9px;
  padding-bottom: 100px;

  @include for-tablet-landscape {
    font-size: 47px;
  }
}
.deliver-text__subtitle {
  margin-top: 75px;

  @include for-tablet-landscape {
    margin-top: 25px;
  }
}
.deliver-subtitle {
  font-family: "Roboto", sans-serif;
  font-size: 38px;
  line-height: 54px;
  color: #fff;

  @include for-tablet-landscape {
    font-size: 30px;
  }
}
.color-text {
  color: #fdc400;
}
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
.deliver-more {
  font-size: 16px;
  line-height: 28px;
  display: flex;
  align-items: center;
  color: #fff;
  font-family: "Roboto", sans-serif;

  @include for-tablet-landscape {
    font-size: 12px;
  }
}
.description {
  max-width: 600px;
  width: 100%;
  box-sizing: border-box;
  text-align: start;
  padding-top: 70px;

  @include for-tablet-landscape {
    padding-top: 40px;
  }
}
.description-title {
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  font-family: "Roboto", sans-serif;

  @include for-tablet-landscape {
    font-size: 12px;
  }
}
</style>