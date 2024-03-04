<script></script>


<template>
    <div class="afisha">
        <div class="container_afisha">
            <h2>АФИША NORI-KARAOKE</h2>
        <div class="card_afisha">
            <div class="imgBx">
                <img src="../../../public/Afisha/slide1.png" alt="">
            </div>
        </div>
        <div class="card_afisha">
            <div class="imgBx">
                <img src="../../../public/Afisha/slide2.png" alt="">
            </div>
        </div>
        <div class="card_afisha">
            <div class="imgBx">
                <img src="../../../public/Afisha/slide3.png" alt="">
            </div>
        </div>
        </div>
    </div>
</template>

<style>
.afisha{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 125vh;
    overflow: hidden;
    padding-top: 150px;
}
.container_afisha h2{
position: absolute;
top: -150px;
left: 15%;
color: azure;
font-size: 50px;
}
.container_afisha{
    position: relative;
    width: 1050px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    transform: skewY(-10deg);
}
.container_afisha .card_afisha{
    transition: 0.5s;
    position: relative;
    width: 300px;
    height: 500px;
}
.container_afisha .card_afisha .imgBx{
    width: 300px;
    height: 380px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    overflow: hidden;
    cursor: pointer;
}
.container_afisha .card_afisha:before{
    content: '';
    position: absolute;
    top: -15px;
    left: 0;
    width: 100%;
    height: 15px;
    background: #000;
    transform-origin: bottom;
    transform: skewX(45deg);
    transition: 0.5s;
}
.container_afisha .card_afisha:after{
    content: '';
    position: absolute;
    top: -15px;
    left: -15px;
    width: 15px;
    height: 76%;
    background: #000;
    transform-origin: left;
    transform: skewY(45deg);
    transition: 0.5s;
}
.container_afisha .card_afisha:hover{
    transform: translateY(-40px);
}
.container_afisha .card_afisha .imgBx img{
    width: 100%;
    height: 100%;
}

</style>