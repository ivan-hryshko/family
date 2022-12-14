<template>
  <div id="app">
    <p>
      Мамуля, вітаємо тебе з Днем народження!!!
    </p>
    <!-- <div class="image-container">
      <svg width="1244" height="957" viewBox="0 0 1244 957" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
        <rect x="193.5" y="7.5" width="1043" height="774" stroke="#D9BEAB" stroke-opacity="0.56" stroke-width="15"/>
        <rect x="7.5" y="175.5" width="1043" height="774" stroke="#D9BEAB" stroke-opacity="0.56" stroke-width="15"/>
        <rect x="48" y="48" width="1148" height="861" fill="url(#pattern0)"/>
        <defs>
        <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
        <use xlink:href="#image0_9_7" transform="scale(0.00078125 0.00104167)"/>
        </pattern>
        </defs>
      </svg>
      <img src="./assets/NY.jpg">
    </div> -->

    <img src="./assets/border/photo1.png">

    <p>
      Найрідніша в світі людина, мила наша матуся
    </p>
    <img src="./assets/border/photo2.png">
    <p>
      Від щирого серця хочемо побажати міцного здоров’я, більше радості кожного дня, позитивних моментів і гарних новин!
    </p>
    <img src="./assets/border/photo3.png">
    <p>
      Ми вас з татом дуже сильно любимо і хочемо щоб ви були самими щасливими!!!
    </p>
    <img src="./assets/border/photo4.png">
    <p>
      Дякуємо вам за неймовірну підтримку, віру, любов, за все, що ви робите для нас
    </p>
    <img src="./assets/border/photo5.png">
    <p id="p-last">
      Дуже сумуємо за вами і з нетерпінням чекаємо зустрічі
    </p>
    <div class="hear-container">
      <svg viewBox="0 0 24 24">
        <path fill="currentColor" d="M12,21.35L10.55,20.03C5.4,15.36 2,12.27 2,8.5C2,5.41 4.42,3 7.5,3C9.24,3 10.91,3.81 12,5.08C13.09,3.81 14.76,3 16.5,3C19.58,3 22,5.41 22,8.5C22,12.27 18.6,15.36 13.45,20.03L12,21.35Z" />
      </svg>
      <svg viewBox="0 0 24 24">
        <path fill="currentColor" d="M12,21.35L10.55,20.03C5.4,15.36 2,12.27 2,8.5C2,5.41 4.42,3 7.5,3C9.24,3 10.91,3.81 12,5.08C13.09,3.81 14.76,3 16.5,3C19.58,3 22,5.41 22,8.5C22,12.27 18.6,15.36 13.45,20.03L12,21.35Z" />
      </svg>
      <svg viewBox="0 0 24 24">
        <path fill="currentColor" d="M12,21.35L10.55,20.03C5.4,15.36 2,12.27 2,8.5C2,5.41 4.42,3 7.5,3C9.24,3 10.91,3.81 12,5.08C13.09,3.81 14.76,3 16.5,3C19.58,3 22,5.41 22,8.5C22,12.27 18.6,15.36 13.45,20.03L12,21.35Z" />
      </svg>
    </div>
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
@import './assets/styles/reset.css';

* {
  box-sizing: border-box;
}

#app {
  font-family: Alice, serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #67443F;
  padding:0px 60px;
  width: 100%;
  background-color: #F0EBE8;
}

p {
  font-size: 60px;
  padding: 300px 0px;
  animation: hear-beat 2s linear infinite alternate 0s forwards;

}

#p-last {
  padding-bottom: 150px;
}


.image-container {
  width: 100%;
  position: relative;
}

.image-container svg{
  width: 100%;
  z-index: 1;
}

.image-container img{
  z-index: 1;
  position: absolute;
  left: 0;
  top: 48px;
  width: calc(100% - 96px);
  /* max-width: 1148px; */
  z-index: 2;
  margin: 0px 48px;
}

img {
  width: 100%;
}

.hear-container {
  display: flex;
  justify-content: center;
}

svg {
  margin-bottom: 150px;
  width: 150px;
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
    font-size: 40px;
    margin: 100px 0px;
  }

  img {
    width: 100%;
  }
}

</style>
