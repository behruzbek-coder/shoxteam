<template>
      <div class="footer">
        <div class="container">
          <div class="content">
            <div class="top">
              <img src="../assets/image/xozufa.svg" alt="" />
              <div class="xoz">
                <img src="../assets/image/xozufa2.svg" alt="" />
                <h6>ХОЗТОВАРЫ С ДОСТАВКОЙ</h6>
              </div>
            </div>
            <div class="bottom">
                <div class="left">
                           
                <h3>Разделы сайта</h3>
                <h3>Каталог товаров</h3>
                <div class="bet">
                      <h3>Контакты</h3>
                </div>
    
              
                </div>
              <div class="right">
                <div class="list">
                <p>Главная</p>
                <p>Акции</p>
                <p>Распродажа</p>
                <p>Оплата и доставка</p>
                <p>Гарантия и возврат</p>
                <p>О нас</p>
                <p>Контакты</p>
    
              </div>
                <div class="list">
                <p>Афганские скороварки </p>
                <p>Казаны и котлы</p>
                <p>Учаги</p>
                <p>Товары для дома и сада</p>
              </div>
                <div class="list">
                <p>Кастрюли</p>
                <p>Мантоварки</p>
                <p>Сковороды</p>
              </div>
              <div class="list">
                <p>Термосы</p>
                <p>Чайники и френч-прессы</p>
                <p>Сервировочная посуда</p>
              </div>
              <div class="list">
                <p>Столовые приборы</p>
                <p>Мантоварки</p>
                <p>Сковороды</p>
              </div>
    
              <div class="list">
                      <p>Революционная 56</p>
                      <p>+7 (347) 276-91-92</p>
                      <span class="email"><img src="../assets/image/email.svg" alt=""><div class="smail"><p>Ежедневно</p><p>10:00-21:00</p></div></span>
                      <span class="email"><img src="../assets/image/info.svg" alt=""><div class="smail"><p>info@newsite.ru</p></div></span>
                </div>
              </div>
                
            </div>
            <div class="last-bottom">
                <div class="list1">
                      <p>Политика компании в отношении обработки </p>
                      <p>персональных данных</p>
                </div>
                <div class="list2">
                      <p>Copyright © 2015-2022. ООО «ХОЗУФА».</p>
                      <p>Все права защищены</p>
                </div>
                <div class="list3">
                      <p>WEBBEES <span>- Создание и продвижение сайтов</span></p>
                </div>
            </div>
          </div>
        </div>
      </div>
    </template>
    
    <script setup>
    </script>
    <style lang="scss" scoped>
    .footer {
      background-color: #333333;
      padding: 10px 0;
      .content {
        display: flex;
        flex-direction: column;
        .top {
          width: 100%;
          display: flex;
          align-items: center;
          justify-content: center;
          border-bottom: 1px solid #fff;
          padding: 7px 0;
          .xoz {
            h6 {
              color: #fff;
            }
          }
        }
        .bottom {
          display: flex;
          gap: 23px;
          flex-direction: column;
          padding: 23px 0;
          .left{
                display: flex;
                gap: 56px;
                .bet{
                      margin-left: auto;
                }
                         h3 {
            width: 156px;
            height: 16px;
            top: 3380.99px;
            left: 100px;
            gap: 0px;
            opacity: 0px;
            color: #fff;
            margin-bottom: 23px;
          }
          }
          .right{
                display: flex;
                align-items: flex-start;
                gap: 103px;
          }
          .list{
                display: flex;
                flex-direction: column;
                gap: 10px;
                .email{
                      display: flex;
                      align-items: center;
                      gap: 10px;
                }
       
          p{
                font-family: SF Pro Display;
                font-size: 14px;
                font-weight: 400;
                line-height: 14px;
                color: #fff;
          }
          }
        }
        .last-bottom{
          display: flex;
          align-items: center;
          justify-content: space-between;
          border-top: 1px solid #fff;
          padding: 10px 0;
          .list1{
                display: flex;
                flex-direction: column;
                gap: 7px;
                p{
                      font-family: Roboto;
                      font-size: 12px;
                      font-weight: 300;
                      line-height: 7.2px;
                      text-align: left;
                      color: #fff;
                      opacity: 0.5;
                }
          }
          .list3{
                display: flex;
                flex-direction: column;
                gap: 7px;
                p{
                      font-family: Roboto;
                      font-size: 12px;
                      font-weight: 300;
                      line-height: 7.2px;
                      text-align: left;
                      color: #fff;
                      span{
                            color: #fff;
                            opacity: 0.5;
                      }
                }
    
          }
          .list2{
                display: flex;
                align-items: center;
                flex-direction: column;
                gap: 7px;
                text-align: center;
                p{
                      font-family: Roboto;
                      font-size: 12px;
                      font-weight: 300;
                      line-height: 7.2px;
                      text-align: left;
                      color: #fff;
                      opacity: 0.5;
                }
          }
        }
      }
    }
    </style>