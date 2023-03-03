<template>
  <body>
    <p class="textCity">Москва</p>
  <div class="imgGradus">
    <img class="weatherImgCity" src="../assets/weather_1.png" alt=""><p class="gradusCity">5</p><p class="gradus">°</p>
  </div>
    <p class="weatherCity">Солнечно</p>
    <p class="days">По дням</p>
        <div class="container_1">
            <div class="item item_1" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Сегодня</p>
                <img class="img_1" src="../assets/weather_1.png" alt="солнечно">
                <p class="d_1">4° <span class="nightGradus">3°</span></p>
            </div>
            <div class="item item_2" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Завтра</p>
                <img class="img_1" src="../assets/weather_2.png" alt="облачно">
                <p class="d_1">19° <span class="nightGradus">6°</span></p>
            </div>
            <div class="item item_3" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Ср 10</p>
                <img class="img_1" src="../assets/weather_3.png" alt="небольшой дождь">
                <p class="d_1">8° <span class="nightGradus">1°</span></p>
            </div>
            <div class="item item_4" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Чт 11</p>
                <img class="img_1" src="../assets/weather_4.png" alt="сильный дождь">
                <p class="d_1">16° <span class="nightGradus">9°</span></p>
            </div>
            <div class="item item_5" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Пт 12</p>
                <img class="img_1" src="../assets/weather_4.png" alt="сильный дождь">
                <p class="d_1">17° <span class="nightGradus">12°</span></p>
            </div>
            <div class="item item_6" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Сб 13</p>
                <img class="img_1" src="../assets/weather_1.png" alt="солнечно">
                <p class="d_1">14° <span class="nightGradus">7°</span></p>
            </div>
            <div class="item item_7" onmouseover="this.style.background='rgba(255,255,255,0.300)';" onmouseout="this.style.background='transparent';"><p class="d1">Вс 14</p>
                <img class="img_1" src="../assets/weather_5.png" alt="дождь с грозой">
                <p class="d_1">10° <span class="nightGradus">11°</span></p>
            </div>
        </div>
        <p class="details">Подробнее</p>
        <hr class="h_line1"><hr class="h_line2">
        <div class="container_2">
            <div class="item_a item__1">По ощущениям <p class="countText">2°</p></div>
            <div class="item_a item__2">Влажность <p class="countText">73%</p></div>
            <div class="item_a item__3">Видимость <p class="countText">10 км</p></div>
            <div class="item_a item__4">Давление <p class="countText">760,00 мм</p></div>
            <div class="item_a item__5">Ветер <p class="countText"><img class="wind" src="../assets/vector.png">4 м/с</p></div>
            <div class="item_a item__6"></div>
        </div>
        <div class="container_3">
            <div class="item_b item___1"><p>Восход</p>
              <img class="sunriseImg" src="../assets/sunrise.png" alt="восход"><span class="timeSun">7:23</span>
            </div>
            <div class="item_b item___2"><p>Закат</p>
              <img class="sunriseImg" src="../assets/sunset.png"  alt="закат"><span class="timeSun">18:42</span>
            </div>
        </div>
  </body>
</template>

<script>
export default {
  name: 'HelloWorld', 
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
* {
  margin: 0px;
  padding: 0px;
  outline: 0px;
  box-sizing: border-box;
}

body {
  font-family: Tahoma;
  /* font-family: 'Roboto'; */
  font-style: normal;
  color: rgb(255, 255, 255);
  background-image: url(../assets/background.jpg);
  background-size: cover;
  background-repeat: no-repeat;
}

button {
 cursor: pointer;
}
.textCity {
  font-size: 20px;
  text-align: center;
  margin-top: 24px;
    position: absolute;
    top: 10px;
    bottom: 0px;
    left: 0px;
    right: 0px; 
}
.d_1 {
  padding-top: 3px;
}
.d1 {
  padding-bottom: 3px;

}
.imgGradus {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 64px;
  position: absolute;
    top: -600px;
    bottom: 0px;
    left: 0px;
    right: 0px; 
}
.weatherImgCity {
  margin-right: 10px;
  height: 70px;
  width: 70px;
}
.gradusCity {
  font-size: 80px;
}
.gradus {
  font-size: 80px;
}
.weatherCity {
  font-size: 20px;
  text-align: center;
  margin-top: 24px;
    position: absolute;
    top: 130px;
    bottom: 0px;
    left: 0px;
    right: 0px; 
}
.nightGradus {
  font-size: 12px;
  color: rgb(191, 191, 191);
}
.days {
  text-align: left;
  margin-left: 64px;
  font-size: 17px;
  position: absolute;
    top: 310px;
    bottom: 0px;
    left: 0px;
    right: 0px;
}
.container_1 {
    display: flex;
    position: absolute;
    top: 350px;
    bottom: 380px;
    left: 0px;
    right: 0px;
    justify-content: space-between;
    justify-items: flex-start;
    flex-wrap: nowrap;
    border: 1px solid rgba(128, 0, 0, 0); /*Граница контейнера*/
    min-height: 120px;
    align-items: center;
    margin-left: 64px;
    margin-right: 64px;
    padding: 0px;
    
}
.item {
  text-align: left;
  font-size: 15px;
  padding: 10px;
  border: 1px solid rgba(0, 250, 154, 0); /*Граница блоков в контейнере*/
  width: 100px;
  height: 110px;
  border-radius: 10px;

}
.item_1 {
  width: 110px;
  height: 110px;
}
.img_1 {
  width: 50px;
  height: 50px;
}
.item_2 {
  width: 110px;
  height: 110px;
}
.item_3 {
  width: 110px;
  height: 110px;

}
.item_4 {
  width: 110px;
  height: 110px;
}
.item_5 {
  width: 110px;
  height: 110px;
}
.item_6 {
  width: 110px;
  height: 110px;
}
.item_7 {
  width: 110px;
  height: 110px;
}


/*Подробнее*/
.details {
  text-align: left;
  margin-left: 64px;
  font-size: 17px;
  position: absolute;
    top: 520px;
    bottom: 0px;
    left: 0px;
    right: 0px;
}

.countText {
  padding-top: 20px;
  font-size: 16px;
}
.h_line1 {
    display: block;
    height: 1px;
    width: 360px;
    border: 0px;
    border-top: 1px solid #ccc;
    margin-left: 64px;
    padding: 0px;
      position: absolute;
      top: 550px;
      bottom: 0px;
      left: 0px;
      right: 0px;
}
.h_line2 {
    display: block;
    height: 1px;
    width: 100px;
    border: 0px;
    border-top: 1px solid #ccc;
    margin-left: 64px;
    padding: 0px;
    position: absolute;
      top: 550px;
      bottom: 0px;
      left: 385px;
      right: 0px;
}


.container_2 {
  display: flex;
  border: 1px solid rgba(255, 0, 0, 0); /*Граница контейнера*/
  min-height: 140px;
  width: 370px;
  justify-content: start;
  justify-items: flex-start;
  flex-wrap: wrap;
  margin-left: 64px;
  margin-bottom: 92px;
  text-align: left;
    position: absolute;
    top: 560px;
    bottom: 380px;
    left: 0px;
    right: 0px;

}
.item_a {
  border: 1px solid rgba(0, 250, 154, 0); /*Граница блоков в контейнере*/
  font-size: 11px;
}
.item__1 {
  width: 120px;
  height: 70px;
}
.item__2 {
  width: 120px;
  height: 70px;
}
.item__3 {
  width: 120px;
  height: 70px;
}
.item__4 {
  width: 120px;
  height: 70px;
}
.wind {
  height: 15px;
  width: 15px;
  margin-right: 10px;
}
.item__5 {
  width: 120px;
  height: 70px;
}
.item__6 {
  width: 120px;
  height: 70px;
}


/*Восход Закат*/
.container_3 {
  display: flex;
  border: 1px solid rgba(128, 0, 0, 0); /*Граница контейнера*/
  min-height: 140px;
  width: 100px;
  text-align: left;
  flex-wrap: wrap;
  margin-left: 64px;
  margin-bottom: 92px;
    position: absolute;
    top: 560px;
    bottom: 0px;
    left: 385px;
    right: 0px;

}
.item_b {
  font-size: 11px;
  align-items: flex-start;
  border: 1px solid rgba(21, 226, 147, 0); /*Граница блоков в контейнере*/
}
.item___1 {
  width: 120px;
  height: 70px;
}
.item___2 {
  width: 120px;
  height: 70px;
}
.sunriseImg {
  margin-top: 10px;
  margin-right: 10px;
  width: 30px;
  height: 30px;
}
.timeSun {
  position: absolute;
  padding-top: 20px;
  font-size: 16px;
}
</style>
