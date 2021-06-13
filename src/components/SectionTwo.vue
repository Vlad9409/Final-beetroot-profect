<template>
  <section class="second" id="second">
    <div class="container">
      <div class="blog-dicsount">
        <h2 class="text-discount">
          Buy a set with a <span class="color-text">30%</span> discount
        </h2>
        <p class="subtitle-discount">
          These baby filters make your drone look faster. Or at least you won’t
          lose them like those other black filters
        </p>
      </div>
      <div class="blog-discount__card">
        <div class="slick" ref="slick">
          <div class="card-one">
            <div class="card-img">
              <img src="/img/card/watch.png" alt="" />
            </div>
            <div class="card-title">
              <h3 class="card-title__name">Fire engine red filters set</h3>
              <h3 class="card-title__description">
                These baby filters make your drone look faster. Or at least you
                won’t lose them like those other black filters
              </h3>
            </div>

            <div class="card-title__price">
              <h3 class="price-real">200 USD</h3>
              <h3 class="price-before">270 USD</h3>
            </div>
            <div class="card-btn">
              <button class="card-buy" value="111001" name="name" type="submit">
                Buy
              </button>
            </div>
          </div>
          <!-- Card 2 -->
          <div class="card-one">
            <div class="card-img">
              <img src="/img/card/camera.png" alt="" />
            </div>
            <div class="card-title">
              <h3 class="card-title__name">Attach ND filters</h3>
              <h3 class="card-title__description">
                Not only do these filters work seamlessly with the camera mounts
                on both Mavic 2 Drones...
              </h3>
            </div>
            <div class="card-title__price">
              <h3 class="price-real">370 USD</h3>
            </div>
            <div class="card-btn">
              <button class="card-buy" value="111001" name="name" type="submit">
                Buy
              </button>
            </div>
          </div>
          <!-- Card 3 -->
          <div class="card-one">
            <div class="card-img">
              <img src="/img/card/kvadrocopter.png" alt="" />
            </div>
            <div class="card-title">
              <h3 class="card-title__name">Drone landing pad</h3>
              <h3 class="card-title__description">
                The helipad that does more for you. Like a changing mat for your
                surf session, the landing pad acts as...
              </h3>
            </div>
            <div class="card-title__price">
              <h3 class="price-real">228 USD</h3>
            </div>
            <div class="card-btn">
              <button class="card-buy" value="111001" name="name" type="submit">
                Buy
              </button>
            </div>
          </div>
          <!-- Card 4 -->
          <div class="card-one">
            <div class="card-img">
              <img src="/img/card/linz.png" alt="" />
            </div>
            <div class="card-title">
              <h3 class="card-title__name">Ultra thin photo case</h3>
              <h3 class="card-title__description">
                Inspired by filmmakers, drone flyers, and minimalists this is
                the case you don’t have to take off to use.
              </h3>
            </div>
            <div class="card-title__price">
              <h3 class="price-real">183 USD</h3>
              <h3 class="price-before">210 USD</h3>
            </div>
            <div class="card-btn">
              <button class="card-buy" value="111001" name="name" type="submit">
                Buy
              </button>
            </div>
          </div>
          <!-- Card 5 -->
          <div class="card-one">
            <div class="card-img">
              <img src="/img/card/linz.png" alt="" />
            </div>
            <div class="card-title">
              <h3 class="card-title__name">Ultra thin photo case</h3>
              <h3 class="card-title__description">
                Inspired by filmmakers, drone flyers, and minimalists this is
                the case you don’t have to take off to use.
              </h3>
            </div>
            <div class="card-title__price">
              <h3 class="price-real">183 USD</h3>
              <h3 class="price-before">210 USD</h3>
            </div>
            <div class="card-btn">
              <button class="card-buy" value="111001" name="name" type="submit">
                Buy
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionTwo",
  mounted() {
    window.$(".slick").slick({
      dots: true,
      slidesToShow: 4,
      slidesToScroll: 1,
      infinite: true,
    });
  },
};
</script>

<style scoped>
h2 {
  margin: 0;
  padding: 0;
}
.color-text {
  color: #fdc400;
}
.second {
  margin: 0 auto;
  padding: 50px 0 0 0;
  max-width: 1440px;
  width: 100%;
  background: #171c1f;
}
.container {
  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
}
.blog-dicsount {
  text-align: start;
  max-width: 595px;
  width: 100%;
  box-sizing: border-box;
}
.text-discount {
  font-size: 38px;
  line-height: 54px;
  color: #fff;
}
.subtitle-discount {
  font-size: 16px;
  line-height: 28px;
  color: #fff;
}
.blog-discount__card {
  display: flex;
  justify-content: space-between;
  padding-top: 60px;
}
.card-one {
  box-sizing: border-box;
  max-width: 272px;
  width: 100%;
}
.card-title {
  max-width: 272px;
  width: 100%;
  padding-top: 40px;
  text-align: start;
}
.card-title__name {
  font-size: 20px;
  line-height: 20px;
  color: #fff;
}
.card-title__description {
  font-size: 14px;
  line-height: 28px;
  color: #fff;
  padding-top: 20px;
}
.card-title__price {
  display: flex;
  flex-direction: row;
}
.price-real {
  text-align: start;
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

.card-btn {
  margin-top: 30px;
}
.card-buy {
  max-width: 272px;
  width: 100%;
  border: 1px solid #fdc400;
  border-radius: 5px;
  padding: 10px 35px;
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  background-color: #161b1e;
}
.card-buy:hover {
  background-color: #fdc400;
}
</style>