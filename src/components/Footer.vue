<template>
  <section class="footer">
    <div class="container">
      <div class="container-menu__footer">
        <div class="logo">
          <a href="#header">
            <img src="../assets/Logofooter.svg" alt="img"
          /></a>
          <h3 class="logo-text">MOMENT OF AIR</h3>
        </div>
        <div class="burder-menu">
          <ul class="burger-container">
            <li class="burger-text__first">
              <a class="burger-title" href="#header">Features</a>
            </li>
            <li class="burger-text">
              <a class="burger-title" href="#header">Tehnoligies</a>
            </li>
            <li class="burger-text">
              <a class="burger-title" href="#header">Who we are</a>
            </li>
            <li class="burger-text">
              <a class="burger-title" href="#header">How do we deliver</a>
            </li>
          </ul>
        </div>
        <div class="btn">
          <a class="buy" href="#1"> Buy a set </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
@import "@/scss/mixin";
.footer {
  margin: 0 auto;
  padding: 0;
  max-width: 1440px;
  width: 100%;
}
.container {
  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
  padding-top: 70px;
}
.logo {
  max-width: 230px;
  width: 200%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  @include for-desktop {
    text-align: center;
    margin: 0 auto;
  }
}
.logo-text {
  font-size: 18px;
  line-height: 28px;
  padding-left: 30px;
  color: #181d20;
  font-family: "Roboto", sans-serif;
}
.container-menu__footer {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
.burger-menu {
  position: absolute;
  box-sizing: border-box;
  max-width: 520px;
  width: 100%;
  margin: 0 165px 0 0;
  padding: 0;
}
.burger-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  text-decoration: none;

  @include for-desktop {
    display: none;
  }
}
.burger-text__first {
  list-style-type: none;
}
.burger-text {
  padding-left: 80px;
  list-style-type: none;
}
.burger-title {
  text-decoration: none;
  color: #181d20;
  font-size: 14px;
  line-height: 20px;
}
.burger-title:hover {
  color: #fdc400;
  border-bottom: 1px solid #fdc400;
}
.buy {
  max-width: 160px;
  width: 100%;
  border: 1px solid #181d20;
  border-radius: 5px;
  padding: 15px 35px;
  font-size: 16px;
  line-height: 28px;
  color: #181d20;
  background-color: #fff;
  text-decoration: none;

  @include for-desktop {
    display: none;
  }
}
.buy:hover {
  color: #fdc400;
  border: 1px solid #fdc400;
}
</style>