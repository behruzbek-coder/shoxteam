<template>
  <div class="sign-up-container">
    <div class="top-of-sign-up">
      <img src="@/assets/image/logo.png" />
      <img src="@/assets/image/close.svg" />
    </div>
    <hr />
    <div class="center-of-sign-up">
      <div class="input-box input-name">
        <label for="name">Имя</label>
        <input type="text" id="name" placeholder="Имя" required/>
      </div>
      <div class="input-box input-name">
        <label for="name">Фамилия</label>
        <input type="text" id="name" placeholder="Фамилия" required/>
      </div>
      <div class="input-box input-name">
        <label for="name">Имя пользователя</label>
        <input type="text" id="name" placeholder="Имя пользователя" required/>
      </div>
      <div class="input-box input-name">
        <label for="name">пароль</label>
        <input type="text" id="name" placeholder="пароль" required/>
      </div>
    </div>

    <div class="bottom-of-sign-up">
      <a href="#" class="forgot">если у вас есть учетная запись</a>

      <button class="button-sign-up">Зарегистрироваться</button>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.sign-up-container {
  width: 500px;
  height: 514px;
  padding: 10px;  
}
.top-of-sign-up {
  display: flex;
  justify-content: space-between;
}

.input-name {
  display: flex;
  flex-direction: column;
}

hr {
  height: 1px;
  width: 100%;
  margin: 10px 0 10px 0;
}

.forgot {
      text-decoration: none;
      margin-top: 4px;
      color: #0094FF;
      font-size: 14px;
}

label {
  font-size: 18px;
}

.input-box {
      margin-top: 10px;
}

input {
  font-size: 18px;
  margin-top: 5px;
  padding: 17px 10px;
}

.button-sign-up {
      margin-top: 20px;
      width: 100%;
      background: #E24C55;
      color: white;
      border: none;
      outline: none;
      padding: 10px 11px;
      font-size: 16px;
}
</style>