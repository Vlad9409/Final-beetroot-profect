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
          <div v-for="(item, index) in slidesData" :key="index">
            <Slidecard v-bind="item" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Slidecard from "./Slidecard.vue";
export default {
  name: "SectionTwo",
  components: {
    Slidecard,
  },
  data() {
    return {
      slidesData: [
        {
          logo: "/img/card/watch.png",
          name: "Fire engine red filters set",
          description:
            "These baby filters make your drone look faster. Or at leastyou won’t lose them like those other black filters",
          price: "200",
          oldprice: "270",
        },
        {
          logo: "/img/card/camera.png",
          name: "Attach ND filters",
          description:
            "Not only do these filters work seamlessly with the cameramounts on both Mavic 2 Drones...",
          price: 370,
        },
        {
          logo: "/img/card/kvadrocopter.png",
          name: "Drone landing pad",
          description:
            "The helipad that does more for you. Like a changing mat for your surf session, the landing pad acts as...",
          price: 228,
        },
        {
          logo: "/img/card/linz.png",
          name: "Ultra thin photo case",
          description:
            "Inspired by filmmakers, drone flyers, and minimalists this isthe case you don’t have to take off to use",
          price: 183,
          oldprice: 210,
        },
        {
          logo: "/img/card/linz.png",
          name: "Ultra thin photo case",
          description:
            "Inspired by filmmakers, drone flyers, and minimalists this isthe case you don’t have to take off to use.",
          price: 183,
          oldprice: 210,
        },
      ],
    };
  },
  mounted() {
    window.$(this.$refs.slick).slick({
      slidesToShow: 4,
      slidesToScroll: 1,
      infinite: true,
      responsive: [
        {
          breakpoint: 1100, // максимальная ширина экрана
          settings: {
            slidesToShow: 3, // показывать по 2 слайда
            slidesToScroll: 1, // скроллить по 2 слайда
          },
        },
      ],
    });
  },
};
</script>

<style lang="scss" scoped>
@import "@/scss/mixin";

.slick-prev:before,
.slick-next:before {
  font-size: 70px;
  color: black;
  left: -100px;
  top: -13px;
  background: white;
  position: absolute;
}
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
  @include for-tablet-landscape {
    padding: 10px 0 0 0;
  }
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
.subtitle-discount {
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  font-family: "Museo Sans Cyrl", sans-serif;

  @include for-tablet-landscape {
    font-size: 12px;
  }
}
.blog-discount__card {
  display: flex;
  justify-content: space-between;
  padding-top: 60px;
}

.slick {
  width: 100%;
  @include for-tablet-landscape {
    width: 1000px;
  }
}
</style>