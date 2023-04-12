<template>
  <div id="app">
      <header id="header">
          <img :src="imagelogo" class="logo">
          <button class="registrate" @click="showModal=true">Regístrate</button>
      </header>
      <div class="part1">
          <div class="part1">
              <img :src="farm1" class="farm">
          </div>
          <div class="parte2">
              <img :src="imagelogo1" class="logo1">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus porttitor fermentum velit,
                  sit amet pulvinar diam suscipit eget. Donec porta mattis felis auctor commodo. Quisque porttitor,
                  est ut rhoncus finibus, ipsum magna vulputate velit, at tempor mi felis in tellus. Praesent condimentum
                  leo in nisi varius tempus. Praesent nec enim eu diam vulputate mollis sed vel metus. Curabitur posuere
                  nunc vitae felis tempus, aliquet fermentum tellus tempor. Aliquam sodales ornare volutpat. Pellentesque
                  turpis nunc, bibendum in nibh gravida, rhoncus convallis arcu. Nam nec purus vehicula, convallis mauris
                  nec, posuere libero. Quisque fermentum mollis nisi et elementum. Curabitur aliquam purus eget.</p>
              <div class="part2.1">
                  <button class="contactanos" @click="showModal=true">Contáctanos</button>
                  <span><a class="video" href="">Ver video</a></span>
              </div>
          </div>
          <div class="part1">
              <img :src="farm2" class="farm">
          </div>
      </div>
      <div>
          <header class="header1">
              <h1>Descubre nuestro beneficios</h1>
          </header>
          <div class="part2">
              <div class="part2">
                  <img :src="farm3" class="farm1" id="box">
                  <div class="box">
                      <h1>Beneficio 1</h1>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                      <a href="">Leer más</a>
                  </div>
              </div>
              <div class="part2">
                  <img :src="farm4" class="farm1">
                  <div class="box">
                      <h1>Beneficio 2</h1>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                      <a href="">Leer más</a>
                  </div>
              </div>
          </div>
          <div class="part2">
              <div class="part2">
                  <img :src="farm5" class="farm2">
                  <div class="box">
                      <h1>Beneficio 3</h1>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                      <a href="">Leer más</a>
                  </div>
              </div>
              <div class="part2">
                  <img :src="farm6" class="farm2">
                  <div class="box">
                      <h1>Beneficio 4</h1>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                      <a href="">Leer más</a>
                  </div>
              </div>
          </div>
      </div>
      <div>
          <header class="header1">
              <h1>Precios</h1>
          </header>
          <div class="part3">
              <div class="part3">
                  <div class="box1">
                      <h1>Para Principiantes</h1>
                      <p>$19</p>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                      <button class="contactanos" @click="showModal=true">Solicitar Demo</button>
                  </div>
              </div>
              <div class="part3">
                  <div class="box1">
                      <h1>Para Equipos</h1>
                      <p>$29</p>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                      <button class="contactanos" @click="showModal=true">Solicitar Demo</button>
                  </div>
              </div>
              <div class="part3">
                  <div class="box1">
                      <h1>Para Compañías</h1>
                      <p>Personalizado</p>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                      <button class="contactanos" @click="showModal=true">Solicitar Demo</button>
                  </div>
              </div>
          </div>
      </div>
      <div class="final">
          <header id="header">
              <div class="part4">
                  <div class="part4">
                      <h2>Lorem ipsum dolor sit amet</h2>
                  </div>
                  <div class="part4">
                      <h2>Recursos</h2>
                      <ul>
                          <li><a href="">Nuestros Agentes</a></li>
                          <li><a href="">Historias de Miembros</a></li>
                          <li><a href="">Video</a></li>
                          <li><a href="">Prueba Gratis</a></li>
                      </ul>
                  </div>
                  <div class="part4">
                      <h2>Compañía</h2>
                      <ul>
                          <li><a href="">Aliados Estratégicos</a></li>
                          <li><a href="">Términos de Uso</a></li>
                          <li><a href="">Privacidad</a></li>
                          <li><a href="">Ayuda</a></li>
                      </ul>
                  </div>
                  <div class="part4">
                      <h2>Mantener Contacto</h2>
                      <ul>
                          <label for="input-text">Ingresa tu email</label>
                          <input type="text" id="input-text" v-model="nombre">
                      </ul>
                  </div>
              </div>
          </header>
      </div>
  </div>
</template>

<!-- SCRIPTS -->
<script>

export default {
  name: 'App',
  data(){
      return{
          showModal: false,
          imageName: 'logo.png',
          imageName1: 'farm.jpg',
          imageName2: 'farm1.png',
          imageName3: 'farm2.jpg',
          nombre: ''
      }
  },
  computed: {
      imagelogo(){
          return require('@/assets/logo.png')
      },
      imagelogo1(){
          return require('@/assets/logo.png')
      },
      farm1(){
          return require('@/assets/img1.jpg')
      },
      farm2(){
          return require('@/assets/img2.jpg')
      },
      farm3(){
          return require('@/assets/img3.png')
      },
      farm4(){
          return require('@/assets/img4.png')
      },
      farm5(){
          return require('@/assets/img5.jpg')
      },
      farm6(){
          return require('@/assets/img6.jpg')
      }
  }
}
</script>

<!-- STYLE-->
<style>
*{
    margin: 0;
    padding: 0;
}
header
{
    background: #FFFBF0;
    padding: 5px;
    display: block;
}
.registrate{
    border: none;
    border-radius: 12px;
    background: #F2858E;
    padding: 15px 20px;
    cursor: pointer;
    display: flex;
    color: white;
    font-size: 18px;
    float: right;
    text-align: center;
    margin: 30px 20px 20px 20px;
}
.contactanos{
    border: none;
    border-radius: 10px;
    background: #F2858E;
    cursor: pointer;
    color : white;
    font-size: 15px;
    padding: 15px 15px;
    text-align: center;
    margin: 10px;
}
.part2.1{
    padding: 10px 20px;
    background-color: #FF6666;
    color: #fff;
    border: none;
    cursor: pointer;
}
.logo{
    width: 350px;
    margin: 0;
    padding: 0;
}

.logo1{
    max-width: 80%;
    text-align: center;
}
.farm{
    width: 100%;
    height: 100%;
    display: flex;
}
.part1{
    width: 1890px;
    height: 450px;
    display: flex;
    padding-top: 30px;
    margin: 0 10px 100px 10px;
    border-radius: 12px;
}
.part1 p {
    margin: 15px;
    text-align-all: center;
}
.part1 span
{
    padding: 10px 20px;
    flex: 0 0 auto;
    margin-left: 10px;
}
.parte2 img
{
    width: 650px;
    text-align: center;
    display: inline-block;
    padding-left: 100px;
}
.part1 span
{
    float: right;
}
header h1
{
    text-align: center;
    background: #FFD8DA;
    font-size: 60px;
}
.part2{
    width: 1690px;
    height: 450px;
    display: flex;
    padding-top: 30px;
    margin: 0 20px 100px 100px;
    border-radius: 12px;
}
.farm1, .farm2
{
    width: 100%;
    height: 100%;
    position: relative;
    margin: 0;
    flex-wrap: wrap;
    box-shadow: black;
}
.part3{
    width: 1690px;
    height: 450px;
    display: flex;
    padding-top: 30px;
    margin: 0 0 0 55px;
    border-radius: 12px;
}
.box
{
    position: absolute;
    text-align: inherit;
    background: linear-gradient(225deg, rgba(186, 251, 227, 0.6) 3.26%, rgba(51, 0, 255, 0.26) 98.18%);
    transform: translateY(274%);
    font-size: 20px;
    height: 120px;
    width: 726px;
}
.box1 {
    background: linear-gradient(225deg, rgba(186, 251, 227, 0.6) 3.26%, rgba(51, 0, 255, 0.26) 98.18%);
    text-align: center;
    height: 320px;
    width: 530px;
    border-radius: 12px;
}
.part3 p{
    font-size: 22px;
    margin:12px;
}
.part3 h1{
    margin: 20px;
}
.part4{
    width: 1690px;
    height: 150px;
    display: flex;
    padding-top: 10px;
    margin: 0 0 0 10px;
}
.part4 ul{
    padding: 30px;
}
.part4 label{
    margin-top: 80px;
}
.part4 input{
    width: 140px;
    height: 20px;
}
</style>
