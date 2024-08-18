<template>
    <div>
        <div class="container">
            <div class="filter_content">
                <h4>Найденно товаров: <span>245</span></h4>
                <div>
                    <input type="checkbox" name="" id="">
                    <h3>Все товары</h3>
                </div>
                <div>
                    <input type="checkbox" name="" id="">
                    <h3>Новинки</h3>
                </div>
                <div>
                    <input type="checkbox" name="" id="">
                    <h3>Со скидкой</h3>
                </div>
                <select name="" id="">
                    <option value="По популярности">По популярности</option>
                    <option value="Сначало дешевле">Сначало дешевле</option>
                    <option value="Сначало дороже">Сначало дороже</option>
                </select>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped> 
        .filter_content{
            width: 100%;
            background: #FFFFFF;
            padding: 12px 39px;
            display: flex;
            margin: 25px 0 25px 0;
            align-items: center;
            justify-content: space-between;
            h4{
                span{
                    font-weight: 900;
                }
            }
            select{
                border: none;
                outline: none;
                option{
                    padding: 10px;
                }
            }
        }
        div{
            display: flex;
            align-items: center;
            gap: 2px;
        }
</style>