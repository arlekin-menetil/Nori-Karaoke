<script setup></script>



<template>
    <div class="banner">
        <div class="container">
        <div class="card">
            <div class="imgBx">
                <img src="../../../public/Gallary/IMG_0639.jpg" alt="">
            </div>
            <div class="contentBx">
                <div class="content">
                    <h2>NORI-KARAOKE</h2>
                    <p>Это уникальное место, где каждый гость может почувствовать себя настоящей звездой. <br> 
                        Вошедший в двери этого заведения, можно окунутся в атмосферу ярких огней и веселья. <br>
                        Мягкое освещение, уютные диванчики и стильный интерьер создают идеальное место для встреч с друзьями или романтических свиданий.
                    </p>
                    <p>
                        Бар предлагает широкий выбор коктейлей и закусок, чтобы поддержать хорошее настроение на весь вечер. <br>
                        Но настоящая звезда шоу - это караоке! Здесь каждый посетитель может исполнить свои <br>
                        любимые хиты на сцене, почувствовать себя настоящей звездой и получить аплодисменты от 
                        восторженной публики
                    </p>
                </div>
            </div>
        </div>
    </div>
    </div>
</template>

 <style>
 .banner{
    width: 100%;
    min-height: 110vh;
    display: flex;
    align-items: center;
    justify-content: center;
 }
 .container{
    position: relative;
    max-width: 1300px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
 }
 .container .card{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    margin: 100px 0;
 }
 .container .card .imgBx{
    position: relative;
    width: 600px;
    height: 400px;
    left: 25px;
    z-index: 1;
 }
 .container .card .imgBx img{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
 }
 .container .card .contentBx{
    position: relative;
    right: 25px;
    width: 500px;
    height: 400px;
    background: linear-gradient(90deg, rgba(0,13,36,1) 0%, rgba(9,53,121,1) 35%, rgba(0,151,255,1) 100% );
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 20px 60px 20px 100px;
    font-weight: bold;
 }
 .container .card .contentBx::before{
    content: '';
    position: absolute;
    top: -50px;
    bottom: -50px;
    left: 0;
    right: 0;
    background: linear-gradient(90deg, rgba(0,13,36,1) 0%, rgba(9,53,121,1) 35%, rgba(0,151,255,1) 100% );
    z-index: -1;
 }
 .container .card .contentBx h2{
    font-size: 30px;
    color: #fff;
 }
 .container .card .contentBx p{
    margin-top: 10px;
    color: #fff;
 }
 /*мобайл верстка*/
@media(max-width: 1000px){
   .container .card{
      flex-direction: column;
      min-width: 350px;
   }
      .container .card .imgBx{
      width: 100%;
      height: 250px;
      left: 0;
   }
   .container .card .contentBx{
      width: 100%;
      height: auto;
      right: 0;
      padding: 30px;
      text-align: center;
   }
   .container .card .contentBx::before{
      top: 0;
      bottom: 0;
   }
}
</style>