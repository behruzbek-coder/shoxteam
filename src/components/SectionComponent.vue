<template>
  <section>
    <div class="container">
      <div class="top">
        <div class="left">
          <img src="../assets/image/Hammasi.png" alt="" />
        </div>
        <div class="bottom">
          <h2>Поможем выбрать лучшее!</h2>
          <img src="../assets/image/22 223.png" alt="" />
          <h1>ХОЗУФА</h1>
          <h4>ХОЗТОВАРЫ С ДОСТАВКОЙ</h4>
        </div>

        <div class="right">
          <h2>Проконсультируем и поможем Вам с выбором!</h2>
          <p>Ваше имя</p>
          <input type="name" />
          <p>Номер телефона</p>
          <input type="password" />
          <button>Получить консультацию</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style lang="scss" scoped>
section {
  background: #fff;
}
.top {
  display: flex;
  align-items: center;
  justify-content: center;
}
.left {
  width: 465.7px;
  height: 269px;
  margin-right: 42.3px;
}
.bottom {
  width: 610px;
  height: 259.07px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  margin-right: 81px;
  h2 {
    height: 29px;
    width: 400px;
    font-family: SF Pro Display;
    font-size: 24px;
    font-weight: 700;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  img{
    margin-bottom: 7px;
    margin-top: 32px;
  }
  h1 {
    width: 281.91px;
    height: 62.65px;
    font-family: Coiny 2;
    font-size: 61.12px;
    font-weight: 400;
    color: #444444;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  h4 {
    width: 281.91px;
    height: 18.48px;
    font-family: SF Pro Display;
    font-size: 19.27px;
    font-weight: 300;
    color: #494949;
    display: flex;
    align-items: center;
    justify-content: center;
  }
}
.right {
  height: 270.02px;
  width: 296.21px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 10px;
  input {
    width: 294px;
    height: 39px;
    top: 3029.99px;
    left: 940px;
    gap: 0px;
    opacity: 0px;
    border: 2px solid #e24c55;
    background: #e8e8e8;
    outline: none;
    padding: 0 10px;
  }
  h2 {
    width: 295.21px;
    height: 45px;
    top: 2944px;
    left: 939.65px;
    gap: 0px;
    opacity: 0px;
    font-family: SF Pro Display;
    font-size: 20px;
    font-weight: 400;
    line-height: 23.87px;
    text-align: center;
    color: #333;
  }
  p {
    width: 113px;
    height: 15px;
    font-family: SF Pro Display;
    font-size: 16px;
    font-weight: 300;
    color: #333;
    display: flex;
    align-items: center;
    justify-content: flex-start;
  }
  button {
    width: 295.21px;
    height: 50px;
    background: #e24c55;
    color: #fff;
    border: none;
    cursor: pointer;
  }
}
</style>