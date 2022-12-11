<template>
  <div id="app">
    <p>
      Мамуля вітаємо тебе з Днем народженя!
    </p>
    <img src="./assets/NY.jpg">
    <p>
      Бажаємо вас всього найкращого
    </p>
    <img src="./assets/bowling.jpg">
    <p>
      Дуже за вами сумуємо
    </p>
    <img src="./assets/kyiv-1.jpg">
    <p>
      Хочемо щоб з вами все було добре
    </p>
    <img src="./assets/kyiv-2.jpg">
    <p>
      З нетерпінням чекаємо на зустріч!
    </p>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  },
}
</script>

<style>
* {
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  padding:0px 60px;
}

p {
  font-size: 60px;
  margin: 300px 0px;
}

img {
  width: 100%;
}

/* #app p:first-child {
  margin: 200px 0px;
} */

</style>
