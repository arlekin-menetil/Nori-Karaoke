<script>
export default {
  data() {
    return {
      videos: [
        { src: '../../../public/News/IMG_7272.mp4' }
        // Добавьте дополнительные объекты с путями к видео, как необходимо
      ]
    };
  }
};
</script>

<template>
    <div class="News_video">
        <h2>НОВОСТИ NORI-KARAOKE</h2>
      <div><video v-for="(video, index) in videos" :key="index" :src="video.src" controls controlsList="nodownload"></video></div>
    </div>
  </template>
  
  <style>
.News_video{
height: 100vh;
width: 100%;
display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
margin-top: 45px;
}
.News_video h2{
    margin: 25px 0 35px 0;
    color: aliceblue;
    font-weight: bold;
}
video{
    width: 350px;
    height: 450px;
}
</style>