<template>
  <header class="header" id="header">
    <div class="container">
      <div class="container-menu">
        <div class="logo">
          <a href="header"> <img src="/img/Logo.svg" alt="img" /></a>
          <h3 class="logo-text">MOMENT OF AIR</h3>
        </div>
        <div class="burder-menu active" id="menu">
          <div class="navigation-menu__burger" id="burger">
            <span></span>
          </div>
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

      <div class="tittle">
        <div class="tittle-text">
          <h1 class="tittle-text__main">ESSENTIAL BLOGGER</h1>
          <div class="tittle-second">
            <h2 class="tittle-text__second">
              Essential lens, filters, and cases for drones
            </h2>
          </div>
          <div class="button-buy">
            <a class="buy-set" href="#">Buy a set</a>
            <span class="buy-quashen">How do we deliver?</span>
            <div class="icon-more">
              <a href="#1" class="more .icon-more">
                <img class="more" src="/img/more.svg" alt="" />
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="position">
      <div class="scroll-container">
        <a href="#second" class="srolls">
          <img class="scroll" src="/img/scroll.svg" alt="" />
        </a>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",

  // data() {
  //   const menu = document.getElementById("menu");
  //   const burger = document.getElementById("burger");

  //   burger.onclick = () => {
  //     menu.classList.toggle("active");
  //   };
  // },
};
</script>

<style lang='scss' scoped>
@import "@/scss/mixin";

.position {
  max-width: 1440px;
  width: 100%;
  height: 90px;
  display: flex;
  justify-content: flex-end;

  @include for-desktop {
    display: none;
  }
}
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
  font-family: "Roboto", sans-serif;
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

  @include for-tablet-landscape {
    margin-left: 20px;
  }
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

  @include for-tablet-landscape {
    padding-left: 40px;
    padding-bottom: 10px;
  }
}
.burger-text {
  padding-left: 80px;
  list-style-type: none;
  z-index: 5;

  @include for-tablet-landscape {
    padding-left: 40px;
    padding-bottom: 10px;
  }
}
.burger-title:hover {
  color: #fdc400;
  border-bottom: 1px solid #fdc400;
}
.burger-title {
  font-family: "Roboto", sans-serif;
  text-decoration: none;
  color: #fff;
  font-size: 14px;
  line-height: 28px;

  @include for-tablet-landscape {
    font-size: 18px;
  }
}
.btn {
  z-index: 10;
}
.buy {
  max-width: 160px;
  width: 100%;
  border: 1px solid #fdc400;
  border-radius: 5px;
  padding: 15px 35px;
  font-size: 16px;
  line-height: 28px;
  color: #fff;
  background-color: #161b1e;
  text-decoration: none;
  z-index: 10;
  font-family: "Roboto", sans-serif;

  @include for-tablet-landscape {
    display: none;
  }
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

  @include for-tablet-landscape {
    font-size: 47px;
  }
  @media (max-width: 727) {
    font-size: 47px;
  }
}
.tittle-second {
  position: relative;
  max-width: 710px;
  width: 100%;
  box-sizing: border-box;
  z-index: 15;
}
.tittle-text__second {
  font-family: "Roboto", sans-serif;
  font-size: 58px;
  color: #fff;
  padding-top: 40px;
  letter-spacing: 3px;
  z-index: 20;

  @include for-tablet-landscape {
    font-size: 30px;
    padding-top: 30px;
  }
  @include for-tablet-portrait {
    font-size: 20px;
  }
}
.button-buy {
  display: flex;
  flex-direction: row;
  align-items: center;
}
.buy-set {
  display: block;
  max-width: 160px;
  border-radius: 5px;
  padding: 12px 35px;
  font-size: 16px;
  line-height: 28px;
  background: #fdc400;
  color: #171717;
  border: 0;
  text-decoration: none;
  z-index: 25;
  font-family: "Roboto", sans-serif;
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
  font-family: "Roboto", sans-serif;
}
.icon-more {
  margin-left: 20px;
  z-index: 35;
}

.more {
  margin-left: 10px;

  @include for-tablet-landscape {
    width: 30px;
  }
}
// .more:hover {
//   box-shadow: -1px -1px 18px 12px rgba(255, 255, 255, 0.2);
// }
.scroll-container {
  display: flex;
  justify-content: center;
  align-items: center;
  // position: relative;
  right: 0;
  max-width: 100px;
  width: 100%;
  height: 100px;
  background-color: #161b1e;

  @include for-tablet-landscape {
    visibility: hidden;
  }

  @include for-tablet-portrait {
    visibility: hidden;
  }
}
// .burder-menu {
//   &__burger {
//     display: none;
//     width: 42px;
//     height: 35px;
//     background-color: transparent;
//     position: relative;
//     z-index: 5;
//     transition: all 0.3s ease-in-out;
//     span {
//       position: absolute;
//       top: 50%;
//       transform: translateY(-50%);
//       width: 100%;
//       height: 4px;
//       background-color: #fff;
//     }
//     &::before,
//     &::after {
//       content: "";
//       position: absolute;
//       width: 100%;
//       height: 4px;
//       background-color: #fff;
//     }
//     &::before {
//       top: 0;
//     }
//     &::after {
//       bottom: 0;
//     }
//     @media (max-width: 767px) {
//       display: block;
//     }
//   }
// }
// @media (max-width: 767px) {
//   .burder-menu .active {
//     .navigation-menu__burger {
//       span {
//         display: none;
//       }
//       &::before {
//         top: 50%;
//         transform: translateY(-50%) rotate(45deg);
//       }
//       &::after {
//         bottom: 50%;
//         transform: translateY(50%) rotate(-45deg);
//       }
//     }
//     .burger-container {
//       display: block;
//       position: absolute;
//       max-width: 767px;
//       width: 100%;
//       min-height: 20vh;
//       top: -18px;
//       right: 0;
//       background-color: rgba(49, 43, 39, 0.9);

//       @media (max-width: 1237px) {
//         .burger-menu__container {
//           max-width: 500px;
//         }
//       }
//     }
//   }
// }
</style>