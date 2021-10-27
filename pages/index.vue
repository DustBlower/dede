<template>
  <div class="container">
    <div class="onePage">
      <a href="https://www.instagram.com/nuas_de.de.de.21/" target="_blank"><div class="insta"></div></a>
      <div class="logo">
        <div class="logoImage"></div>
        <div class="type"></div>
      </div>
          <div class="main">
          </div>
      </div>
    <div class="pageList">
    <div class="twoPage">
          <p class="aboutTitle">で!De!デ!とは？？</p>
          <p class="aboutText">このデザイン学科有志による学祭は初めての試みであり、今まで学祭を経験したことのないメンバーによって構成されています。<br>「Enjoy！」をテーマに作る側も見る側も楽しく、を意識した企画となっています！<br>また、大学での対面を基礎とした構成になっていますが、オンラインでも楽しんで頂けるように作業過程の動画や完成品の写真を掲載しています！</p>
          </div>
        </div>
      <div class="threePage">
            <p class="linksTitle">LINKS</p>
            <div class="projectList">
              <div class="buppan"><nuxt-link to="zoukei"><a href="https://www.instagram.com/nuas_de.de.de.21/"><img src="~assets/img/mikoshi.jpg"></a></nuxt-link></div>
              <div class="rippoutai"><nuxt-link to="comd"><a href="https://www.instagram.com/nuas_de.de.de.21/"><img src="~assets/img/rippoutai.png"></a></nuxt-link></div>
              <div class="communicationd"><nuxt-link to="comd"><a href="https://nuas-design-exhibition.com/communicationdesign"><img src="~assets/img/commd.png"></a></nuxt-link></div>
            </div>
          </div>
      <div class="fourPage">
            <div class="contactBall">
              <div class="contactTitleBox">
                <p class="contactTitle">CONTACT</p>
                </div>
              <div class="nuas">NUAS: <a href="https://www.nuas.ac.jp/">https://www.nuas.ac.jp/</a> </div>
              <div class="nuas2">INSTAGRAM: <a href="https://www.instagram.com/nuas_de.de.de.21/">nuas_de.de.de.21</a> </div>
            </div>
          </div> 
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
  $initBack: #020223;
  $mainText: #363636;
  $subText: #7b7b7b;
  $Dred: #EC6B4D;
  $Dyellow:#FDD800;
  $Dblue:#00B7D6;
.container {
  overflow: hidden;
  font-family: 'Noto Sans JP', sans-serif;
  .onePage{
    position: relative;
    height: calc(100vh + 1px);
    width: 100%;
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
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
    .logo{
      height: 100vh;
      width: 100vw;
      z-index: 3;
      position: absolute;
      top: 0px;bottom: 0;left: 0;right: 0;
      margin: auto;
      overflow: hidden;
      text-align: center;
      .logoImage{
        margin-top:40px;
        background: url("assets/img/logo2.svg") no-repeat center;
        height: 70%;
        width: auto;
        animation: initLogo 1s  1s forwards;
        transform: scale(0) rotate(-180deg);
      }
      .type{
        background: url("assets/img/type.svg") no-repeat center;
        height: 10%;
        width: auto;
        animation: initType 0.6s 2.1s forwards;
      }
    }
  }
  .twoPage{
    width: 100%;
    height: 100%;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    color: $mainText;
    .aboutTitle{
      color: $Dred;
      margin-top: 10vh;
      padding: 15px;
      z-index: 3;
      border-radius: 15px;
      font-size: 22px;
      font-weight:bold;
      border:6px solid $Dred;
      padding-bottom: 18px;
    }
    .aboutText{
      font-size: 16px;
      width: 70%;
      margin-top: -50px;
      padding:50px;
      overflow-wrap:break-word;
      border-radius: 15px;
      z-index: 2;
      padding-top:60px;
      color:black;
    }
  }
  .threePage{
      height: 100%;
      margin-top: 250px;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    .linksTitle{
        color: rgb(255, 111, 0);
        padding: 15px;
        font-size: 20px;
        border-radius: 15px;
        font-size: 22px;
        font-weight:bold;
        border:6px solid $Dyellow;
        padding-bottom: 18px;
    }
      .projectList {
        margin-top: 68px;
        div {
          width: 80%;
          display: inline-block;
          vertical-align: top;
          margin: 5px 20px 20px 0;
          height: 300px;
          width: 300px;
          background-size: cover;
          transition: transform 1s ease;
          overflow: hidden;
          transition: scale 0.4s ease;
            &:nth-child(1) {
              border:15px solid $Dred;
              img{
                cursor: pointer;
                transition: scale 0.4s ease;
                transition: filter 0.4s ease;
                height: 300px;
                filter: grayscale(100%);
                transform: scale(1);
                &:hover{
                  transform: scale(1.05);
                  filter: grayscale(0%);
                }
              }
            }
            &:nth-child(2) {
              border:15px solid $Dyellow;
              img{
                cursor: pointer;
                height: 300px;
                filter: grayscale(100%);
                transition: filter 0.4s ease;
                &:hover{
                  transform: scale(1.05);
                  filter: grayscale(0%);
                }
              }
            }
            &:nth-child(3) {
              border:15px solid $Dblue;
              img{
                cursor: pointer;
                height: 300px;
                filter: grayscale(100%);
                transition: filter 0.4s ease;
                &:hover{
                  transform: scale(1.05);
                  filter: grayscale(0%);
                }
              }
            }
          }
        }
  }
  .fourPage{
    width: 100%;
    margin-top: 280px;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    color: $mainText;
    .contactBall{
      margin-bottom: -450px;
      height: 800px;
      width: 800px;
      border-radius: 50%;
      border: 15px solid $Dblue;
      z-index: 0;
      .contactTitleBox{
        width: 100px;
        margin: 0 auto;
      }
      .nuas{
        margin-top:70px;
      }
      .nuas2{
        margin-top:40px;
      }
    }
    .contactTitle{
      border-bottom: 1px solid $subText;
      margin-top: 50px;
      padding: 8px;
      font-size: 20px;
    }
  }
}
  @keyframes initLogo {
    0%{transform: scale(0) rotate(-180deg)}
    40%{transform: scale(1.1) rotate(20deg);}
    100%{transform: scale(1) rotate(0deg);}
  }
    @keyframes initType {
    0%{transform: scale(1)}
    40%{transform: scale(1.1)}
    100%{transform: scale(1)}
  }
</style>