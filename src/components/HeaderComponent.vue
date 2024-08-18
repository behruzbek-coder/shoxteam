<template>
  <div class="container">
    <div class="top">
      <div class="botom">
        <div class="left">
          <div>
            <img src="../assets/image/Group.png" alt="" />
            <h4>Большой асортимент <span>и выбор товаров</span></h4>
          </div>
          <div>
            <img src="../assets/image/Group (1).png" alt="" />
            <h4>Предлогаем только <span>качественные товары</span></h4>
          </div>
        </div>
        <div class="left">
          <div>
            <img src="../assets/image/Group (2).png" alt="" />
            <h4>Работаем напрямую <span> с производителями</span></h4>
          </div>
          <div>
            <img src="../assets/image/Group (3).png" alt="" />
            <h4>Предоставляем гарантию <span> на все товары</span></h4>
          </div>
        </div>
        <div class="left">
          <div>
            <img src="../assets/image/Group (4).png" alt="" />
            <h4>Бесплатная доставка <span> товаров на дом</span></h4>
          </div>
          <div>
            <img src="../assets/image/Group (6).png" alt="" />
            <h4>Безопастная система <span> онлайн-оплаты</span></h4>
          </div>
        </div>
      </div>
      <div class="right">
        <h2>Продажа казанов и котелков с дочтавкой на дом!</h2>
      </div>
    </div>
  </div>
</template>
    
    <script setup>
</script>
    
    <style lang="scss" scoped>
.top {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: #fff;
  gap: 80px;
  .botom {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-left: 30px;
    width: 393px;
    height: 378px;
    .left {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 30px;
      div {
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        margin-bottom: 20px;
        h4 {
          flex-wrap: wrap;
          text-align: center;
          font-family: SF Pro Display;
          font-size: 14px;
          font-weight: 500;
          color: #565656;
        }
      }
    }
  }
}
.right {
  background-repeat: no-repeat;
  width: 920px;

  height: 378px;
  background: linear-gradient(180deg, #000000 0%, rgba(0, 0, 0, 0) 50%),
    url("../assets/image/3 154371.png");
  h2 {
    width: 741px;
    height: 31px;
    font-family: SF Pro Display;
    font-size: 28px;
    font-weight: 700;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 10px;
    color: #fff;
  }
}
</style>