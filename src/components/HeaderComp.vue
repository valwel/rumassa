<template>
  <div class="header">

    <div class="header__top container">
      <div class="header__top-logo">
        <img src="@/assets/logo.svg" alt="">
        <div class="header__top-logo-title">Интернет-магазин <br> RU-massa</div>
      </div>
      <div class="header__top-search">
        <div class="header__top-search-input-wrapper">
          <input class="header__top-search-input" type="text" placeholder="Поиск">
          <img class="header__top-search-icon small-img" src="@/assets/search.svg" alt="">
        </div>
      </div>

      <div class="header__top-links">
        <div class="header__top-link">
          <img class="small-img" src="@/assets/mail.svg" alt="">
        </div>
        <div class="header__top-link">
          <img class="small-img" src="@/assets/tg.svg" alt="">
        </div>
      </div>
    </div>

    <div class="header__bottom">
      <div class="header__bottom-content container">
        <button class="header__catalogue-button">
          <img class="header__catalogue-button-icon small-img" src="@/assets/more.svg" alt="">
          Каталог
        </button>

        <nav class="header__nav">
          <ul class="header__nav-list">
            <li class="header__nav-item">Оральные препараты</li>
            <li class="header__nav-item">Инъекционные препараты</li>
            <li class="header__nav-item">Препараты ПКТ</li>
            <li class="header__nav-item">Гормон роста</li>
            <li class="header__nav-item">Сармы/Sarms</li>
          </ul>
        </nav>

        <div class="header__actions">
          <ul class="header__actions-list">
            <li class="header__actions-item"><img class="small-img" src="@/assets/user.svg" alt=""></li>
            <li class="header__actions-item">
              <img class="small-img" src="@/assets/graph.svg" alt="">
              <div class="counter">0</div>
            </li>
            <li class="header__actions-item">
              <img class="small-img" src="@/assets/heart.svg" alt="">
              <div class="counter">0</div>
            </li>
            <li class="header__actions-item">
              <img class="small-img" src="@/assets/shoping-cart.svg" alt="">
              <div class="header__actions-item-shoping">
                <div class="header__actions-item-shop">
                  0 ₽
                </div>
                <div class="header__actions-item-shop">
                  0 товаров
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>



  </div>
</template>

<script>
export default {
  name: 'header-comp'
}
</script>

<style lang="scss">
.counter {
  background-image: url(@/assets/counter.svg);
  background-repeat: no-repeat;
  width: 17px;
  height: 15px;
  position: absolute;
  margin-right: -44px;
  margin-top: -36px;
  font-size: 10px;
  color: #fff;
  display: flex;
  align-items: center;
  justify-content: center;
}

.container {
  max-width: 1380px;
  width: 100%;
  margin: 0 auto;
}

.small-img {
  max-width: 30px;
  max-height: 30px;
}

.header {
  // display: flex;
  // justify-content: center;

  &__top {
    // border-bottom: 1px solid #d3d3d3;
    display: flex;
    width: 100%;
  }

  &__top-logo {
    display: flex;
    align-items: center;
    padding-right: 65px;
  }

  &__top-logo-title {
    margin-left: 11px;
    font-size: 18px;
    font-weight: bold;
  }

  &__top-search {
    flex-grow: 1;
    padding: 18px 31px;
    border-left: 1px solid #d3d3d3;
    border-right: 1px solid #d3d3d3;
  }

  &__top-search-input-wrapper {
    position: relative;
    display: flex;
  }

  &__top-search-input {
    background: transparent;
    outline: none;
    border: 1px solid #d3d3d3;
    width: 100%;
    padding: 17px 80px 17px 20px;

  }

  &__top-search-icon {
    position: absolute;
    width: 20px;
    height: 20px;
    right: 21px;
    top: 15px;
  }

  &__top-links {
    display: flex;
    align-items: center;
    padding-left: 21px;
  }

  &__top-link {
    width: 50px;
    height: 50px;
    border: 1px solid #d3d3d3;
    display: flex;
    align-items: center;
    justify-content: center;

    &:nth-child(n+2) {
      margin-left: 10px;
    }
  }

  &__bottom {
    border-top: 1px solid #d3d3d3;
    border-bottom: 1px solid #d3d3d3;
  }

  &__bottom-content {
    display: flex;
  }

  &__catalogue-button {
    padding: 13px 15px;
    display: flex;
    align-items: center;
    border: 0;
    outline: none;
    background: linear-gradient(130.83deg, #CFAE87 9.11%, #A48159 70.56%);
    color: #fff;
    min-width: 156px;
    cursor: pointer;
    font-size: 16px;
    line-height: 20px;
  }

  &__catalogue-button-icon {
    margin-right: 11px;
  }

  &__nav {
    padding-left: 39px;
  }

  &__nav-list {
    display: flex;
    margin: 0;
    padding: 0;

  }

  &__nav-item {
    font-size: 14px;
    line-height: 18px;
    padding: 19px 15px;
  }

  &__actions {
    margin-left: auto;
    margin-right: 0;
  }

  &__actions-list {
    display: flex;
  }

  &__actions-item {
    width: 55px;
    height: 55px;
    border-left: 1px solid #d3d3d3;
    display: flex;
    align-items: center;
    justify-content: center;

    &:nth-child(4) {
      width: 115px;
      border-right: 1px solid #d3d3d3;
    }
  }

  &__actions-item-shoping {
    padding-left: 10px;
  }

  &__actions-item-shop {
    font-size: 12px;

    &:nth-child(2) {
      color: #A4A4A4;
    }
  }
}
</style>