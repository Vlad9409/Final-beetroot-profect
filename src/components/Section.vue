<template>
  <section class="section1">
    <div class="container">
      <div class="blog-photo">
        <img class="photo-section" src="/img/section1.png" alt="" />
        <img class="photo-logo" src="/img/Logo.svg" alt="" />
      </div>
      <div class="blog-text">
        <h2 class="blog-text__title">ESSENTIAL</h2>
        <div class="blob-text__subtitle">
          <h2 class="text-subtitle">
            Essential <span class="color-text">blogger</span> accessories and
            <span class="color-text">filmmaker’s</span> tool
          </h2>
        </div>
        <p class="blog-description">
          We put our prototypes in the hands of our favorite drone flyers and
          filmmakers. What they captured in a few days blew our minds. We can't
          wait to see what you capture with this gear.
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Section",
};
</script>

<style scoped>
.section1 {
  margin: 0 auto;
  padding: 0;
  max-width: 1440px;
  width: 100%;
  background: #171c1f;
  padding-bottom: 123px;
}
.container {
  display: flex;
  flex-direction: row;

  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
  padding-top: 160px;
}
.color-text {
  color: #fdc400;
}
.blog-text__title {
  position: absolute;
  color: #fff;
  opacity: 0.05;
  font-size: 75px;
  line-height: 1px;
  letter-spacing: 9px;
  padding-bottom: 100px;
}
.blob-text__subtitle {
  position: relative;
  padding-top: 20px;
  max-width: 574px;
}
.text-subtitle {
  font-size: 40px;
  line-height: 54px;
  color: #fff;
}
.blog-description {
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  letter-spacing: 1px;
}
.blog-text {
  max-width: 662px;
  width: 100%;
  text-align: start;
  box-sizing: border-box;
  margin-left: 98px;
}
.photo-section {
  max-width: 500px;
  width: 100%;
  height: 350px;
}
.photo-logo {
  position: relative;
  bottom: 370px;
  left: 220px;
  width: 70px;
  height: 70px;
}
</style>
