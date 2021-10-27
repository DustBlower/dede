<template>
  <div class="zoukei">
    <a href="https://www.instagram.com/nuas_de.de.de.21/" target="_blank"><div class="insta"></div></a>
    <h1 class="omTitle">ワンマンスチャレンジ</h1>
  <video src="../assets/video.mp4" class="kaboM" autoplay muted controls></video>
    <!-- <div class="movie">
        <iframe class="videoM"  src="https://www.youtube.com/embed/gb6RcazTL0o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div> -->
</div>
</template>

<script>
export default {
  components: {
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP&display=swap');
$Dred: #EC6B4D;

.zoukei {
    font-family: 'Noto Sans JP', sans-serif;
    position: relative;
    height: 100vh;
    width: 100%;
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    .omTitle{
      top: 0vh;
      color:$Dred;
      font-size: 80px;
    }
    .insta{
      position: fixed;
      top:30px;
      right:30px;
      height: 50px;
      width: 50px;
      background:url("assets/img/instaRGB.png")no-repeat;
      background-size: cover;
      cursor: pointer;
      z-index: 5;
    }
    .kaboM{
      top: 20vh;
      border:15px solid $Dred;
      height: 70vh;
      width: 70vw;
      display: block;
    }
    .movie{
      width: 100%;
    .videoM{
      height: 800px;
      width: 80%;
    }
    }
  }
</style>