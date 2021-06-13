<template>
  <header class="header" id="header">
    <div class="container">
      <div class="container-menu">
        <div class="logo">
          <a href="header"> <img src="/img/Logo.svg" alt="img" /></a>
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
          <button class="buy" value="111001" name="name" type="submit">
            Buy a set
          </button>
        </div>
      </div>

      <div class="tittle">
        <div class="tittle-text">
          <h1 class="tittle-text__main">ESSENTIAL BLOGGER</h1>
          <div class="tittle-second">
            <h2 class="tittle-text__second">
              Essential lens, filters, and cases for drones
            </h2>
          </div>
          <div class="button-buy">
            <button class="buy-set">Buy a set</button>
            <span class="buy-quashen">How do we deliver?</span>
            <div class="icon-more">
              <a href="#" class="more .icon-more">
                <img class="more" src="/img/more.svg" alt="" />
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="scroll-container">
      <a href="#second" class="srolls">
        <img class="scroll" src="/img/scroll.svg" alt="" />
      </a>
    </div>
    <!-- <div class="fon"></div>
    <div class="fon2"></div> -->
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.header {
  margin: 0 auto;
  padding: 0;
  max-width: 1440px;
  width: 100%;

  background: url(../assets/background.png) no-repeat;
}

.logo {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
.logo-text {
  font-size: 18px;
  line-height: 28px;
  padding-left: 30px;
  color: #fff;
}
.container {
  margin: 0 auto;
  max-width: 1240px;
  width: 100%;
  padding-top: 50px;
}

.container-menu {
  position: relative;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
.burger-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  text-decoration: none;
  margin-left: 100px;
}
.burger-menu {
  position: absolute;
  box-sizing: border-box;
  max-width: 515px;
  width: 100%;
  margin: 0 auto;
}
.burger-text__first {
  list-style-type: none;
}
.burger-text {
  padding-left: 80px;
  list-style-type: none;
  z-index: 5;
}
.burger-title:hover {
  color: #fdc400;
  border-bottom: 1px solid #fdc400;
}
.burger-title {
  text-decoration: none;
  color: #fff;
  font-size: 14px;
  line-height: 28px;
}
.btn {
  z-index: 10;
}
.buy {
  max-width: 160px;
  width: 100%;
  border: 1px solid #fdc400;
  border-radius: 5px;
  padding: 10px 35px;
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  background-color: #161b1e;
  z-index: 10;
}
.buy:hover {
  background-color: #fdc400;
}
.fon {
  position: relative;
  display: flex;
  justify-content: flex-end;
  right: 0;
  left: 925px;
  top: -633px;
  max-width: 515px;
  width: 100%;
  height: 322px;
  background-color: #161b1e;
}
.fon2 {
  position: relative;
  display: flex;
  justify-content: flex-end;
  right: 0;
  top: -550px;
  max-width: 515px;
  width: 100%;
  height: 322px;
  background-color: #161b1e;
}

.tittle {
  margin-top: 250px;
}
.tittle-text {
  max-width: 973px;
  width: 100%;
  text-align: start;
  box-sizing: border-box;
}
.tittle-text__main {
  position: absolute;
  color: #fff;
  opacity: 0.05;
  font-size: 75px;
  line-height: 1px;
  letter-spacing: 9px;
  z-index: 15;
}
.tittle-second {
  position: relative;
  max-width: 710px;
  width: 100%;
  box-sizing: border-box;
  z-index: 15;
}
.tittle-text__second {
  font-size: 58px;
  color: #fff;
  padding-top: 40px;
  letter-spacing: 3px;
  z-index: 20;
}
.button-buy {
  display: flex;
  flex-direction: row;
  align-items: center;
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
  z-index: 25;
}
.buy-set:hover {
  background: #fcde7b;
}
.buy-quashen {
  font-size: 16px;
  color: #fff;
  line-height: 28px;
  margin-left: 40px;
  z-index: 30;
}
.icon-more {
  margin-left: 20px;
  z-index: 35;
}
.more:hover {
  box-shadow: -1px -1px 18px 12px rgba(54, 164, 249, 0.2);
}
.scroll-container {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  left: 1340px;
  right: 0;
  max-width: 100px;
  width: 100%;
  height: 100px;
  background-color: #161b1e;
}
</style>