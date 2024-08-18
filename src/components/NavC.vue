<template>
  <div>
    <nav>
      <div class="container">
        <div class="nav_contact">
          <div class="nav_left">
          <div class="nav_logo">
            <img src="../images/22 224.png" alt="" />
            <div class="nav_logo_titles">
              <h2>ХОЗУФА</h2>
              <h4>ХОЗТОВАРЫ С ДОСТАВКОЙ</h4>
            </div>
          </div>
          <button class="nav_btn">
            <div class="bars">
              <span class="bars_1"></span>
              <span class="bars_2"></span>
              <span class="bars_3"></span>
            </div>
            Каталог товаров
          </button>
          <div class="nav_inputs">
            <input
              type="text"
              placeholder="Введите артикул или название товара..."
              class="nav_input"
            />
            <img src="../images/magnifying-glass 1.png" alt="" />
          </div>
        </div>
        <div class="nav_right">
          <div class="nav_pro">
            <div class="wk">
              <img src="../images/image 378.png" alt="">
            </div>
            <div class="tg">
              <img src="../images/Vector.png" alt="">
            </div>
            <div class="wh">
              <img src="../images/Vector (1).png" alt="">
            </div>
          </div>
          <div class="nav_icons">
            <div class="like">
              <img src="../images/Group 5783.png" alt="">
            </div>
            <div class="shop">
              <img src="../images/22222 1.png" alt="">
            </div>
            <button class="nav_btn">Зарегистрироваться</button>
          </div>
        </div>
        </div>
      </div>
    </nav>
    <nav>
      <div class="container">
        <div class="nav_bottom">
          <ul class="nav_list">
            <li>Главная</li>
            <li>Акции</li>
            <li>Распродажа</li>
            <li>Оплата и доставка</li>
            <li>Гарантия и возврат</li>
            <li>О нас</li>
            <li>Контакты</li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Coiny&family=Jost:ital,wght@0,100..900;1,100..900&display=swap");

nav {
  display: flex;
  align-items: center;
}

.nav_left {
  display: flex;
  align-items: center;
  .nav_logo {
    display: flex;
    align-items: center;
    cursor: pointer;
    .nav_logo_titles {
      h2 {
        font-family: "Coiny", sans-serif;
        font-size: 32.86px;
        font-weight: 700;
        line-height: 36.14px;
        text-align: center;
      }
      h4 {
        font-size: 9.99px;
        font-weight: 400;
        line-height: 11.92px;
        text-align: center;
      }
    }
  }
  .nav_btn {
    font-size: 16px;
    font-weight: 700;
    color: #fff;
    text-align: left;
    gap: 14px;
    border: 2px solid transparent;
    padding: 10px 16px;
    margin-left: 40px;
    display: flex;
    background: #e24c55;
    transition: .3s;
    cursor: pointer;
    &:hover {
      background: #fff;
      color: #e24c55;
      border: 2px solid #e24c55;
    }
    &:active {
      background: #e24c568e;
    }
    &:hover span {
      background: #e24c55;
      color: #e24c55;
    }
    span {
      width: 25px;
      height: 2px;
      background-color: #fff;
    }
    .bars {
      gap: 5px;
      display: flex;
      flex-direction: column;
    }
  }
}

.nav_inputs {
  display: flex;
  align-items: center;
  width: 318px;
  margin-left: 29px;
  height: 40px;
  background: #ececec;
  border: 2px solid #adadad;
  .nav_input {
    border: none;
    background: #ececec;
    outline: none;
    font-size: 14px;
    font-weight: 400;
    line-height: 16.41px;
    width: 100%;
    text-align: left;
    padding-left: 10px;
  }
  img {
    padding: 10px;
    border-left: 2px solid #adadad;
    cursor: pointer;
  }
}

.nav_right{
  display: flex;
  align-items: center;
  .tg{
    background: #27ACC9;
    border-radius: 50%;
    padding-top: 8px;
    padding-left: 2px;
    width: 42px;
    height: 42px;
  }
  .wh{
    background: #48C162;
    border-radius: 50%;
    width: 42px;
    height: 42px;
    padding-top: 7px;
    padding-left: 7.5px;
  }
  .nav_pro{
    display: flex;
    align-items: center;
    gap: 15px;
  }
  .nav_icons{
    display: flex;
    align-items: center;
    gap: 15px;
    .like{
      border: 2px solid #C0C0C0;
      width: 42px;
      height: 42px;
      border-radius: 50%;
      text-align: center;
      margin-left: 10px;
      padding-top: 8px;
      padding-left: 2px;
    }
    .shop{
      border: 2px solid #C0C0C0;
      width: 42px;
      height: 42px;
      border-radius: 50%;
      text-align: center;
      padding-top: 8px;
    }
  }
  .nav_btn{
    background: #e24c55;
    padding: 12px 8px;
    border: 2px solid transparent;
    border-radius: 8px;
    cursor: pointer;
    transition: .3s;
    color: #fff;
    &:hover {
      background: #fff;
      color: #e24c55;
      border: 2px solid #e24c55;
    }
    &:active {
      background: #e24c568e;
    }
  }
}

.nav_contact{
  display: flex;
  align-items: center;
}

nav{
  background: #fff;
  border-bottom: 1px solid #D7D7D7;
  padding-bottom: 2px;
}

.nav_bottom{
  padding: 22px;
  .nav_list{
    display: flex;
    justify-content: space-between;
    list-style: none;
    li{
      font-size: 14px;
      font-weight: 600;
      line-height: 16.41px;
      text-align: left;
      color: #000;
      font-family: sans-serif;
      cursor: pointer;
    }
  }
}
</style>