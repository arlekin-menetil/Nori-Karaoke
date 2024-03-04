<script>

</script>



<template>
    <div class="News_gallary">
        <div class="container">
            <div class="box">
                <div class="imgBx">
                    <img src="../../../public/News/Instagram post - 1199.png" alt="">
                </div>
            </div>
            <div class="box">
                <div class="imgBx">
                    <img src="../../../public/News/Instagram post - 1201 (2).png" alt="">
                </div>
            </div>
            <div class="box">
                <div class="imgBx">
                    <img src="../../../public/News/Instagram post - 1201.png" alt="">
                </div>
            </div>
            <div class="box">
                <div class="imgBx">
                    <img src="../../../public/News/Обложка.png" alt="">
                </div>
            </div>
            <div class="box">
                <div class="imgBx">
                    <img src="../../../public/News/Премиум 2023.png" alt="">
                </div>
            </div>
            <div class="box">
                <div class="imgBx">
                    <img src="../../../public/News/Спешл 2023.png" alt="">
                </div>
            </div>
            <div class="box">
                <div class="imgBx">
                    <img src="../../../public/News/Стандартт.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>



<style>
.News_gallary{
    display: flex;
    width: 100%;
    height: 150vh;
    justify-content: center;
    padding-top: 30px;
}
.container{
    position: absolute;
    display: flex;
    height: calc(100% - 200px);
    width: calc(100% - 200px);
    z-index: 100;
}
.container .box{
    position: relative;
    width: 25%;
    height: 100%;
    overflow: hidden;
    border-bottom: 1px solid #000;
    border-right: 1px solid #000;
}
.container .box:nth-child(4),
.container .box:last-child{
    border-right: none;
}
.container .box .imgBx{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    transition: 0.5s;
    opacity: 0.5;
    filter: grayscale(1);
}
.container .box .imgBx{
position: fixed;
top: 100px;
left: 100px;
height: calc(100% - 200);
}
.container .box .imgBx:hover{
    opacity: 1;
    filter: grayscale(0);
}
.container .box .imgBx img{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
}
</style>