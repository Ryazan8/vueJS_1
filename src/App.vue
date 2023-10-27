<script>
  export default {
    data() {
      return{
        menu: document.querySelector('.btn-1'),
        header: document.querySelector('.btn-2'),
        content: document.querySelector('.btn-3'),
        footer: document.querySelector('.btn-4'),
      }
    },
    methods: {
      menuClick() {
        this.menu = document.querySelector('.menu-none').style.display = 'block'
      },
      headerClick() {
        this.header = document.querySelector('.header-none').style.display = 'block'
      },
      contentClick() {
        this.content = document.querySelector('.content').style.display = 'block'
      },
      footerClick() {
        this.footer = document.querySelector('.footer').style.display = 'block'
      },

    }
  }

</script>

<template>
  <div class="site">
    <div class="buttons">
      <div @click="menuClick" class="btn btn-1"><a href="#">Menu</a></div>
      <div @click="headerClick" class="btn btn-1"><a href="#">Header</a></div>
      <div @click="contentClick" class="btn btn-1"><a href="#">Content</a></div>
      <div @click="footerClick" class="btn btn-1"><a href="#">Footer</a></div>
    </div>

    <div class="container">

      <div class="menu-none">
        <div class="menu">
          <a href="#" class="menu-link">Каталог</a>
          <a href="#" class="menu-link">О нас</a>
          <a href="#" class="menu-link">Контакты</a>
        </div>
      </div>

      <div class="header-none">
        <div class="header">
          <div class="header-text">
            <h1>Главный текст!</h1>
            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. </p>
          </div>
          <div class="header-btn"><a href="#" class="header-btn-link">Кнопка</a></div>
        </div>
      </div>


        <div class="content">
          <div class="content-title">
            <h1>Заглавие</h1>
          </div>
          <div class="boxes">
            <div class="box"></div>
            <div class="box"></div>
            <div class="box"></div></div>
        </div>



      <div class="footer"></div>
    </div>
  </div>


</template>

<style>

*{
  padding: 0;
  margin: 0;
}

.site{
  display: flex;
}

  .container{
    width: 100%;
    max-width: 1500px;
    margin: 0 auto;
  }

  .menu-none{
    display: none;
  }

  .menu{
    display: flex;
    justify-content: center;
    background-color: rebeccapurple;
  }

  .menu-link{
    text-decoration: none;
    color: #ffffff;
    padding: 25px 50px 25px 0;
  }

  .header-none{
    display: none;
  }

  .header{
    display: flex;
    padding-top: 50px;
    background-color: indigo;
    padding-bottom: 50px;
  }

  .header-text{
    max-width: 400px;
    color: #ffffff;
    padding-left: 450px;
  }

  .header-text h1{
    font-size: 40px;
    padding-bottom: 20px;
  }

  .header-btn{
    padding-left: 80px;
    padding-top: 50px;
  }
  .header-btn-link{
    color: #fff;
    text-decoration: none;
    font-size: 20px;
    font-weight: bold;
    padding: 5px 10px;
    border-radius: 6px;
    background-color: seagreen;
  }

  .content{
    display: none;
    background: blueviolet;
  }

  .content-title {
    padding-top: 50px;
  }

  .content-title h1{
    font-size: 30px;
    text-align: center;
    color: #ffffff;
  }

  .boxes{
    padding-top: 50px;
    display: flex;
    justify-content: center;
  }

  .box{
    height: 100px;
    width: 100px;
    margin-right: 25px;
    background-color: #c9c9c9;
    margin-bottom: 50px;
  }

  .footer{
    display: none;
    height: 100px;
    background-color: mediumpurple;
  }

  .buttons{
    margin: 15px 0 0 15px;
  }

  .buttons a{
    color: #fff;
    text-decoration: none;
    font-size: 20px;
    font-weight: bold;
    padding: 5px 10px;
    border-radius: 6px;
    background-color: seagreen;
  }

  .btn{
    margin-bottom: 15px;
  }


</style>