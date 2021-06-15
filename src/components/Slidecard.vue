<template>
  <div class="card-one">
    <div class="card-img">
      <img :src="logo" alt="" />
    </div>
    <div class="card-title">
      <h3 class="card-title__name">{{ name }}</h3>
      <h3 class="card-title__description">
        {{ description }}
      </h3>
    </div>
    <div class="card-title__price">
      <h3 class="price-real">{{ price }} USD</h3>
      <h3 v-if="oldprice" class="price-before">{{ oldprice }} USD</h3>
    </div>
    <div class="card-btn">
      <a class="card-buy" href="#"> Buy </a>
    </div>
  </div>
</template>

<script>
export default {
  props: ["logo", "name", "description", "price", "oldprice"],
};
</script>

<style lang="scss" scoped>
@import "@/scss/mixin";
.card-one {
  box-sizing: border-box;
  max-width: 272px;

  @include for-tablet-landscape {
    max-width: 200px;
  }
}
.card-title {
  max-width: 272px;
  width: 100%;
  padding-top: 40px;
  text-align: start;

  @include for-tablet-landscape {
    max-width: 200px;
  }
}
.card-title__name {
  font-family: "Roboto", sans-serif;
  font-weight: 600;
  font-size: 20px;
  line-height: 20px;
  color: #fff;

  @include for-tablet-landscape {
    font-size: 16px;
  }
}
.card-title__description {
  font-family: "Museo Sans Cyrl", sans-serif;
  font-weight: 300;
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
  font-family: "Museo Sans Cyrl", sans-serif;
  text-align: start;
  font-size: 20px;
  line-height: 24px;
  color: #fff;

  @include for-tablet-landscape {
    font-size: 16px;
  }
}
.price-before {
  font-family: "Museo Sans Cyrl", sans-serif;
  font-weight: 300;
  line-height: 24px;
  text-decoration-line: line-through;
  color: #afafaf;
  margin-left: 40px;

  @include for-tablet-landscape {
    font-size: 16px;
    margin-left: 20px;
  }
}
.card-btn {
  margin-top: 30px;
  max-width: 272px;
  width: 100%;

  @include for-tablet-landscape {
    max-width: 200px;
  }
}
.card-buy {
  text-decoration: none;
  display: block;
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