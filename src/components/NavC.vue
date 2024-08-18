<template>
  <div>
    <nav>
      <div class="container">
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
    line-height: 19.09px;
    text-align: left;
    gap: 14px;
    border: 2px solid transparent;
    padding: 10px 16px;
    margin-left: 58px;
    display: flex;
    background: #e24c55;
    cursor: pointer;
    &:hover{
      background: #fff;
      color: #e24c55;
      border: 2px solid #e24c55;
    }
    &:hover span{
      background: #e24c55;
      color: #e24c55;
    }
    span{
      width: 25px;
      height: 2px;
      background-color: #fff;
    }
    .bars{
      gap: 5px;
      display: flex;
      flex-direction: column;
    }
  }
}
</style>