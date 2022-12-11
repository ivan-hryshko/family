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
    <svg style="width:300px;height:300px" viewBox="0 0 24 24">
      <path fill="currentColor" d="M12,21.35L10.55,20.03C5.4,15.36 2,12.27 2,8.5C2,5.41 4.42,3 7.5,3C9.24,3 10.91,3.81 12,5.08C13.09,3.81 14.76,3 16.5,3C19.58,3 22,5.41 22,8.5C22,12.27 18.6,15.36 13.45,20.03L12,21.35Z" />
    </svg>
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
  width: 100%;
}

p {
  font-size: 60px;
  margin: 300px 0px;
  animation: hear-beat 2s linear infinite alternate 0s forwards;

}

img {
  width: 100%;
  border: 20px solid #931b05;
  border-radius: 10px;
}

svg {
  margin-bottom: 150px;
}

svg path {
  fill: #931b05;
  /* animation: hear-beat 1.5s linear infinite alternate 0s forwards; */
  animation-name: hear-beat;
  animation-duration: 1.5s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
  animation-fill-mode: forwards;

}

#app p {
  margin-bottom: 200px;
}

@keyframes hear-beat {
  0% {
    fill: transparent;
  }
  100% {
    fill: #931b05;
  }
}

@media (max-width: 1000px) {

  #app {
    padding:0px 20px;
  }

  p {
    font-size: 60px;
    margin: 150px 0px;
  }

  img {
    width: 100%;
    border: 10px solid #931b05;
    border-radius: 10px;
  }
}

</style>
