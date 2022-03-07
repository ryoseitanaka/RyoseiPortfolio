<template>
  <div class="body">
    <div class="Firstview">
      <div class="Firstview__Img">
        <h1 class="Firstview__Text">
          In the<br />
          shape of<br />
          <span>excitement</span>
        </h1>

        <header class="header">
          <nav>
            <ul class="header__Items">
              <li class="header__Item"><a href="">ABOUT</a></li>
              <li class="header__Item"><a href="">PROFILE</a></li>
              <li class="header__Item"><a href="">WORKS</a></li>
              <li class="header__Item"><a href="">CONTACT</a></li>
            </ul>
          </nav>
        </header>
      </div>
    </div>
    <main class="main">
      <div class="About">
        <h2 class="title About__Title">ABOUT</h2>
        <h3 class="About__Subtitle">わくわくを一緒に創り上げる</h3>
        <p class="About__Text">
          子供の頃は新しい発見が沢山あり、わくわくする毎日でした。<br />
          新しい発見を形にし関わる人と一緒にわくわくすることが、自分の揺るがない軸です。
        </p>
      </div>
      <div class="About__Wrap">
        <!-- <iframe
          class="About__Iframe"
          src="http://127.0.0.1:5500/index.html"
          width="100%"
          height="100%"
          frameborder="0"
        ></iframe> -->
      </div>

      <div class="Profile">
        <h2 class="title Profile__Title">PROFILE</h2>
        <div class="Profile__Img">
          <div class="Profile__Info">
            <h3 class="Profile__Name">
              田中 凌生<br /><span>tanaka ryosei</span>
            </h3>
            <h4 class="Profile__School">
              ECCコンピュータ専門学校<br />
              マルチメディア研究学科 Webデザインコース<br /><span
                >2023卒業予定</span
              >
            </h4>
            <p class="Profile__Detail">
              キャリアプランとしてフロントエンドを経て<br />
              Webディレクターになり、一緒にわくわくを創り上げていきたいです。<br />
              趣味は好きなアーティストのライブに行くことです。
            </p>
          </div>
        </div>
      </div>
      <div class="Works">
        <h2 class="title Wroks__Title">WORKS</h2>
        <div class="Works__List">
          <ul class="Works__Items">
            <li class="Works__Item Pikup">
              <a href="">
                <img src="../assets/pickup-1.png" alt="" />
              </a>
            </li>
            <li class="Works__Item">
              <a href="">
                <img src="../assets/work-4.png" alt="" />
              </a>
            </li>
            <li class="Works__Item">
              <a href="">
                <img src="../assets/work-3.png" alt="" />
              </a>
            </li>
            <li class="Works__Item">
              <a href="">
                <img src="../assets/work-2.png" alt="" />
              </a>
            </li>
            <li class="Works__Item">
              <a href="#">
                <img src="../assets/work-1.png" alt="" />
              </a>
            </li>
          </ul>
          <div class="Works__Btn"><a href="#">作品をもっとみる</a></div>
        </div>
      </div>
      <div class="Contact">
        <h2 class="title Contact__Title">CONTACT</h2>
        <p class="Contact__Text">お気軽にご連絡ください</p>
        <address class="Contact__Address">
          <p>ryoseitanaka12@gmail.com</p>
        </address>
        <div class="Contact__Sns">
          <a href="#"><img src="../assets/Twitter-logo.svg" alt="" /></a
          ><a href="#"><img src="../assets/Instagram-logo.svg" alt="" /></a
          ><a href="#"><img src="../assets/GitHub-logo.svg" alt="" /></a>
        </div>
      </div>
    </main>
    <footer class="footer">
      <p>RyoseiTanaka</p>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css2?family=Anton&family=Noto+Sans+JP:wght@100;300;400;500;700;900&display=swap");
body {
  font-family: "Anton", "Noto Sans JP", sans-serif;
}

@import url("../scss/_ress.scss");
@import url("../scss/_var.scss");
$mainColor: #212121;
$subColor: #03a2ff;
$accentColor: #ff8637;

.body {
  background: $mainColor;
  color: #fff;
  //   font-family: "Anton", "Noto Sans JP", sans-serif;フォントがわからない
}
.Firstview {
  &__Img {
    background-image: url(../assets/Firstview.png);
    background-size: cover;
    height: 100%;
    width: 100%;
    // filter: brightness(50%);
  }

  height: 100vh;
  width: 100vw;

  &__Text {
    padding-top: 50px;
    padding-left: 150px;
    color: #fff;
    font-size: 140px;
    line-height: 155px;
    text-align: left;

    mix-blend-mode: screen;
    span {
      color: $accentColor;
    }
  }
  .header {
    display: block;
    nav {
      display: flex;
      justify-content: center;
      margin: 83px;
    }
    &__Items {
      height: 70px;
      width: 450px;
      border-radius: 5px;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: rgba(29, 29, 29, 0.75);
    }
    &__Item {
      list-style: none;
      color: #fff;
      font-size: 18px;
      margin: 0 20px;
    }
    a {
      color: #fff;
      text-decoration: none;
    }
  }
}
.main {
  .title {
    color: $subColor;
    font-size: 32px;
    margin-bottom: 32px;
  }
  .About {
    margin-top: 150px;
    &__Subtitle {
      font-size: 32px;
      margin-bottom: 16px;
    }
    &__Text {
      font-size: 16px;
    }

    &__Iframe {
      height: 100%;
    }
  }
  .Profile {
    margin-top: 150px;
    &__Img {
      height: 520px;
      background-image: url(../assets/Profile_img.png);
      background-size: cover;
      display: flex;
      justify-content: end;
      align-items: center;
      padding-right: 188px;
    }
    &__Name {
      text-align: left;
      font-size: 40px;
      line-height: 25px;

      span {
        // display: inline;
        color: $subColor;
        font-size: 22px;
        // margin-right: 13px;
      }
    }
    &__School {
      font-family: "Noto Sans JP", sans-serif;

      //   padding-left: 235px;
      text-align: left;
      font-size: 20px;
      margin: 30px 0 25px 0;
      span {
        font-size: 16px;
      }
    }
    &__Detail {
      font-family: "Noto Sans JP", sans-serif;

      // display: inline;
      //   padding-left: 235px;
      text-align: left;
      font-size: 16px;
    }
  }
  .Works {
    margin-top: 150px;
    a {
      display: block;
      text-decoration: none;
    }

    &__Items {
      padding: 0 50px;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }
    &__Item {
      width: 580px;
      height: 350px;
      list-style: none;
      margin: 20px 22.5px;
      img {
        height: 100%;
        width: 100%;
      }
    }
    .Pikup {
      height: 420px;
      width: 1220px;
    }
    &__Btn {
      height: 60px;
      width: 300px;
      margin: 50px auto 0 auto;
      background-color: $mainColor;
      border: $accentColor solid 1px;
      border-radius: 5px;
      text-align: center;
      line-height: 60px;
      a {
        display: block;
        border-radius: 5px;
        color: $accentColor;
        font-size: 18px;
        font-weight: bold;
        transition: 0.3s;
      }
      & a:hover {
        background-color: $accentColor;
        color: $mainColor;
        // border: $accentColor solid 1px;
      }
    }
  }
}
.Contact {
  margin-top: 150px;

  &__Text {
    font-size: 20px;
  }
  &__Address {
    font-size: 32px;
    color: $accentColor;
  }
  &__Sns {
    display: flex;
    justify-content: center;
    align-items: center;
    a {
      margin: 30px;
    }
  }
}

.footer {
  margin-top: 150px;
  color: #fff;
  font-size: 18px;
  height: 80px;
  width: 100%;
  text-align: center;
  line-height: 80px;
  letter-spacing: 1px;
  background-color: $subColor;
}
</style>

<script>
// const Text = (elment, sentence) => {
//   [...sentence].forEach((character, index) => {
//     setTimeout(() => {
//       document.querySelector(elment).textContent += character;
//     }, 100 * ++index);
//   });
// };

// Text("#Text", "In the shape of excitement");
</script>
