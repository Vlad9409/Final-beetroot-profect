<template>
  <section class="oneclick">
    <div class="container">
      <div class="block-one">
        <img class="photo-one" src="/img/mirrow.png" alt="" />
      </div>
      <div class="click-text">
        <div class="click-text__block">
          <h2 class="click-text__title">
            Just make <span class="color-text">one click</span> and we will send
            you our set!
          </h2>
          <div class="price">
            <h3 class="price-real">200 USD</h3>
            <h3 class="price-before">270 USD</h3>
          </div>
          <button class="buy-set">Buy a set</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Oneclick",
};
</script>

<style scoped>
.color-text {
  color: #fdc400;
}
.oneclick {
  margin: 0 auto;
  padding: 0;
  padding-top: 50px;
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
.photo-one {
  max-width: 560px;
  width: 100%;
  height: 362px;
}
.click-text {
  width: 500px;
  text-align: start;
  box-sizing: border-box;
  margin-left: 92px;
}
.click-text__title {
  font-size: 40px;
  line-height: 54px;
  letter-spacing: 0.02em;
  color: #ffffff;
  margin: 0;
  padding-bottom: 15px;
}
.price {
  display: flex;
  flex-direction: row;
  margin: 0;
  padding-bottom: 15px;
}
.price-real {
  font-size: 20px;
  line-height: 24px;
  color: #fff;
}
.price-before {
  font-size: 20px;
  line-height: 24px;
  text-decoration-line: line-through;
  color: #afafaf;
  margin-left: 40px;
}
.buy-set {
  max-width: 160px;
  width: 100%;
  border-radius: 5px;
  padding: 10px 35px;
  font-size: 16px;
  line-height: 28px;
  background: #fdc400;
  color: #171717;
  border: 0;
}
.buy-set:hover {
  background: #fcde7b;
}
</style>