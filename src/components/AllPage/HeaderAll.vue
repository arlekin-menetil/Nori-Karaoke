<script>
export default {
  mounted() {
    let lastScrollTop = 0;
    let navbar = document.getElementById("navbar");
    window.addEventListener("scroll", () => {
      let scrollTop = window.pageYOffset || document.documentElement.scrollTop;
      if (scrollTop > lastScrollTop) {
        navbar.classList.add("icon");
      } else {
        navbar.classList.remove("icon");
      }
      lastScrollTop = scrollTop;
    });
  }
}
</script>



<template>
    <div class="hederall">
        <div id="navbar">
            <a href="#" class="brand">
                <span><img  style="width: 50px; height: 50px;" src="../../../public/icons/logo_white.PNG" /></span>
                <span><img src="../../../public/icons/logo_black.PNG" /></span>
            </a>
            <ul>
                <li style="--i:0;">
                    <a href="/">
                        <span>Главная</span>
                        <span><img style="width: 30px; height: 30px" src="../../../public/icons/home-outline.svg" alt=""></span>
                    </a>
                </li>
                <li style="--i:1;">
                    <a href="#">
                        <span>Меню</span>
                        <span><img style="width: 30px; height: 30px" src="../../../public/icons/food.svg" alt=""></span>
                        </a>
                </li>
                <li style="--i:2;">
                    <a href="#">
                        <span>Афиша</span>
                        <span><img style="width: 30px; height: 30px" src="../../../public/icons/afisha.svg" alt=""></span>
                    </a>
                </li>
                <li style="--i:3;">
                    <a href="#">
                        <span>Сотрудничество</span>
                        <span><img style="width: 30px; height: 30px" src="../../../public/icons/people-circle-outline.svg" alt=""></span>
                        </a>
                </li>
                <li style="--i:4;">
                    <a href="#">
                        <span>Галерея</span>
                        <span><img style="width: 30px; height: 30px" src="../../../public/icons/gallary.svg" alt=""></span>
                    </a>
                </li>
                <li style="--i:5;">
                    <a href="/news">
                        <span>Новости</span>
                        <span><img style="width: 30px; height: 30px" src="../../../public/icons/news.svg" alt=""></span>
                    </a>
                </li>
            </ul>
            <Span>
                <li>Режим работы</li>
                <li>17:00-05:00</li>
            </Span>
        </div>
    </div>
</template>


<style>
.hederall{
    color: #fff;
    width: 100%;;
}
.hederall div:first-child{
    background: #fff;
}
#navbar{
    position: fixed;
    top: 0;
    width: 100%;
    height: 80px;
    padding: 0 50px;
    transition: 0.5s;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 1000;
}
#navbar ul{
    display: flex;
}
#navbar ul li{
    margin-right: 10px;
}
#navbar ul li a{
position: relative;
color: #444;
padding: 5px 20px;
font-size: 1.1em;
font-weight: bold;
display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
overflow: hidden;
}
 ul li a span{
    transition: 0.5s;
    transition-delay: calc(0.05s * var(--i));
    }
 ul li a span:last-child{
    position: absolute;
    transform: translateY(35px);
        }
.icon ul li a:first-child span{
    transform: translateY(-30px);
    }
.icon ul li a span:nth-child(2){
        transform: translateY(2px);
            }
#navbar span{
    color: #444;
    text-align: center;
    font-weight: bold;
}
/*animation logo*/
.brand{
    position: relative;
    padding: 0 5px;
    overflow: hidden;
}
.brand span{
    transition: 0.5s;
    display: block;
}
.brand span{
    width: 100px;
    height: 50px;
}
.brand span img{
    width: 100%;
}
.brand span:nth-child(1){
    position: absolute;
    transform: translateY(-80px);
}
.icon .brand span:first-child{
    transform: translateY(0px);
}
.icon .brand span:last-child{
    transform: translateY(55px);
}

</style>