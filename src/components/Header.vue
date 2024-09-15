<script setup></script>

<template>
  <div class="body_wraper">
    <header class="header">
      <img src="../assets/img/Blurr.svg" class="effect-banner" />
      <div class="container">
        <div id="menu" class="animate__animated animate__fadeInDown">
          <div class="logo">
            <img src="/favicon.png" alt="logo" />
          </div>
          <input type="checkbox" id="burger-checkbox" class="burger-checkbox" />
          <label class="burger" for="burger-checkbox"></label>
          <ul class="menu open">
            <li>
              <a href="#">Explore</a>
            </li>
            <li>
              <a href="#">Creators</a>
            </li>
            <li>
              <a href="#">Community</a>
            </li>
          </ul>
          <button class="connect">Connect Wallet</button>
        </div>
        <div class="content">
          <div class="left animate__animated animate__fadeInLeft">
            <div class="effect_one"></div>
            <div class="title">
              Explore, Buy and <br />
              Sell the
              <span
                >Best <br />
                NFTs!</span
              >
            </div>
            <button class="one-bt">Explore</button>
            <button class="two-bt">Create</button>
            <div class="numbers">
              <div class="one">
                <h1>32k+</h1>
                <p>Artworks</p>
              </div>
              <div class="two">
                <h1>20k+</h1>
                <p>Auctions</p>
              </div>
              <div class="three">
                <h1>12k+</h1>
                <p>Creators</p>
              </div>
            </div>
          </div>
          <div class="right">
            <div class="banner">
              <div class="timer">
                <div class="current-bid">
                  <p>Current Bid</p>
                  <h1>0.99 ETH</h1>
                </div>
                <div class="ends">
                  <p>Ends in</p>
                  <h1>25 hrs</h1>
                </div>
              </div>
              <div class="user">
                <div class="artist">
                  <h4>Artist</h4>
                  <p>@wzard</p>
                </div>
                <button>Start Bid</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<style>
.burger-checkbox {
  display: none;
}
.burger {
  display: none;
}
.menu-icon {
  display: none;
}

header {
  position: relative;
  z-index: 1000;
  top: 0;
  width: 100%;
  display: flex;
  justify-content: center;
  .effect-banner {
    position: absolute;
    z-index: -1;
    width: 770px;
    height: 1063px;
    top: 0;
    right: 0;
    margin-left: 1140px;
    backdrop-filter: blur(30px);
    background: rgba(79, 70, 78, 0.45);
  }
  .container {
    width: 1367px;
    #menu {
      display: flex;
      padding-top: 25px;
      .menu {
        display: flex;
        padding-top: 17px;
        margin-left: 565px;
        /* margin-right: 64px; */
        li {
          margin-right: 64px;
          padding-bottom: 20px;
          transition: all 1s ease;
          a {
            color: var(--white-two);
            font-size: 18px;
            font-family: "Work Sans", sans-serif;
          }
          @media (hover: hover) {
            :hover {
              color: #ffce4e;
              padding-bottom: 5px;
              border: 2px solid #ffce4e;
              border-width: 0 0 2px;
            }
          }
          @media (hover: none) {
            :hover {
              color: #ffce4e;
              padding-bottom: 5px;
              border: 2px solid #ffce4e;
              border-width: 0 0 2px;
            }
          }
        }
        .close {
          display: none;
        }
      }
      .connect {
        /* margin-left: 75px; */
        background: rgba(233, 215, 167, 0.1);
        color: var(--gold-five);
        font-family: "Work Sans", sans-serif;
        font-size: 18px;
        font-weight: 700;
        padding: 22px 30px;
        border: 1px solid var(--gold-five);
        transition: all 0.2s ease;
      }

      @media (hover: hover) {
        .connect:hover {
          box-shadow: inset 0 0 0 2em var(--gold-five);
          color: #f5fbf2;
        }
      }
      @media (hover: none) {
        .connect:active {
          box-shadow: inset 0 0 0 2em var(--gold-five);
          color: #f5fbf2;
        }
      }
    }
    .content {
      padding-top: 140px;
      display: flex;
      justify-content: center;
      .effect_one {
        position: absolute;
        z-index: -1;
        width: 202px;
        height: 208px;
        filter: blur(250px);
        background: rgba(231, 178, 38, 0.8);
        transform: rotate(5deg);
        left: 0;
        top: 450px;
      }
      .title {
        position: relative;
        z-index: 1;
        padding-top: 20px;
        font-family: "Oxanium", sans-serif;
        font-weight: 700;
        font-size: 85px;
        line-height: 130px;
        line-height: 1.52941;
        color: #f5fbf2;
        span {
          color: var(--gold-five);
        }
      }
      .one-bt {
        padding: 24px 76px;
        margin-top: 77px;
        background: var(--gold-five);
        font-family: "Work Sans", sans-serif;
        font-weight: 600;
        font-size: 28px;
        line-height: 36px;
        line-height: 1.28571;
        color: #000;
        transition: all 0.2s ease;
      }
      @media (hover: hover) {
        .one-bt:hover {
          box-shadow: inset 9em 0 0 0 var(--white-three);
          color: var(--gold-five);
        }
      }
      @media (hover: none) {
        .one-bt:active {
          box-shadow: inset 9em 0 0 0 var(--white-three);
          color: var(--gold-five);
        }
      }
      .two-bt {
        padding: 24px 76px;
        margin-top: 77px;
        margin-left: 48px;
        background: rgba(233, 215, 167, 0.1);
        border: 1px solid var(--gold-five);
        font-family: "Work Sans", sans-serif;
        font-weight: 600;
        font-size: 28px;
        line-height: 36px;
        line-height: 1.28571;
        color: #fff;
        transition: all 0.2s ease;
      }
      @media (hover: hover) {
        .two-bt:hover {
          box-shadow: inset 9em 0 0 0 var(--gold-five);
          color: var(--black);
        }
      }
      @media (hover: none) {
        .two-bt:active {
          box-shadow: inset 9em 0 0 0 var(--gold-five);
          color: var(--black);
        }
      }
      .numbers {
        display: flex;
        margin-top: 80px;
        .one {
          margin-left: 40px;
          h1 {
            font-family: "Work Sans", sans-serif;
            font-weight: 700;
            font-size: 64px;
            line-height: 96px;
            line-height: 1.5;
            color: var(--white-two);
          }
          p {
            font-family: "Work Sans", sans-serif;
            font-weight: 400;
            font-size: 18px;
            line-height: 27px;
            line-height: 1.66667;
            color: #8613a5;
            padding-left: 21px;
          }
        }
        .two {
          margin-left: 103px;
          h1 {
            font-family: "Work Sans", sans-serif;
            font-weight: 700;
            font-size: 64px;
            line-height: 96px;
            line-height: 1.5;
            color: var(--white-two);
          }
          p {
            font-family: "Work Sans", sans-serif;
            font-weight: 400;
            font-size: 18px;
            line-height: 27px;
            line-height: 1.66667;
            color: #8613a5;
            padding-left: 21px;
          }
        }
        .three {
          margin-left: 103px;
          h1 {
            font-family: "Work Sans", sans-serif;
            font-weight: 700;
            font-size: 64px;
            line-height: 96px;
            line-height: 1.5;
            color: var(--white-two);
          }
          p {
            font-family: "Work Sans", sans-serif;
            font-weight: 400;
            font-size: 18px;
            line-height: 27px;
            line-height: 1.66667;
            color: #8613a5;
            padding-left: 21px;
          }
        }
      }
      .right {
        margin-left: 10%;
      }
      .banner {
        position: relative;
        width: 100%;
        height: 100%;
        background: url(../assets/img/nft-1.png);
        background-size: auto 100%;
        /* background-position: 50% 50%; */
        background-repeat: no-repeat;
        z-index: 1;
        padding-top: 24px;
        .timer {
          display: flex;
          /* width: 512px;
          height: 98px; */
          padding-top: 18px;
          padding-left: 40px;
          padding-bottom: 18px;
          /* padding-right: 40px; */
          margin-left: 22px;
          margin-right: 22px;
          backdrop-filter: blur(45px);
          box-shadow: 0 4px 30px 0 rgba(0, 0, 0, 0.12);
          background: var(--oreng);
          opacity: 0.95;
          .current-bid {
            p {
              font-family: "Oxanium", sans-serif;
              font-weight: 500;
              font-size: 18px;
              letter-spacing: 0.08em;
              text-transform: capitalize;
              color: var(--white-three);
            }
            h1 {
              margin-top: 7px;
              font-family: "Oxanium", sans-serif;
              font-weight: 700;
              font-size: 32px;
              color: #fff;
            }
          }
          .ends {
            margin-left: 182px;
            p {
              font-family: "Oxanium", sans-serif;
              font-weight: 500;
              font-size: 18px;
              letter-spacing: 0.08em;
              text-transform: capitalize;
              color: var(--white-three);
            }
            h1 {
              margin-top: 7px;
              font-family: "Oxanium", sans-serif;
              font-weight: 700;
              font-size: 32px;
              color: #fff;
            }
          }
        }
        .user {
          display: flex;
          width: 590px;
          height: 142px;
          margin-top: 506px;
          padding-top: 33px;
          backdrop-filter: blur(27px);
          background: #b5c8db;
          .artist {
            margin-left: 60px;
            h4 {
              font-family: "Oxanium", sans-serif;
              font-weight: 600;
              font-size: 28px;
              letter-spacing: 0.07em;
              color: #16091b;
            }
            p {
              font-family: "Work Sans", sans-serif;
              font-weight: 400;
              font-size: 24px;
              line-height: 35px;
              line-height: 1.47717;
              color: var(--gray-four);
            }
          }
          button {
            width: 205px;
            height: 72px;
            margin-left: 160px;
            font-family: "Work Sans", sans-serif;
            backdrop-filter: blur(45px);
            background: var(--gold-five);
            font-weight: 700;
            font-size: 24px;
            color: #000;
          }
        }
      }
    }
  }
}

@media (max-width: 1662px) {
  header {
    .container {
      #menu {
        padding-top: 40px;
        .connect {
          font-size: 15px;
        }
      }
      .content {
        padding-top: 100px;
        .title {
          font-size: 68px;
        }
        .one-bt {
          font-size: 24px;
        }
        .two-bt {
          font-size: 24px;
        }
        .numbers {
          .one {
            h1 {
              font-size: 54px;
            }
          }
          .two {
            h1 {
              font-size: 54px;
            }
          }
          .three {
            h1 {
              font-size: 54px;
            }
          }
        }
      }
    }
  }
}

@media (max-width: 1456px) {
  header {
    .effect-banner {
      width: 600px;
      height: 971px;
    }
  }
}

@media (max-width: 1380px) {
  header {
    .container {
      #menu {
        margin-left: 50px;
        .menu {
          margin-left: 465px;
        }
      }
      .left {
        margin-left: 50px;
        .title {
          font-size: 58px;
        }
        .one-bt {
          font-size: 20px;
        }
        .two-bt {
          font-size: 20px;
        }
      }
      .content {
        .numbers {
          .one {
            margin-left: 0px;
            h1 {
              font-size: 34px;
              margin-left: 25px;
            }
          }
          .two {
            margin-left: 73px;
            h1 {
              font-size: 34px;
              margin-left: 25px;
            }
          }
          .three {
            margin-left: 73px;
            h1 {
              font-size: 34px;
              margin-left: 25px;
            }
          }
        }
      }
    }
  }
}

@media (max-width: 1276px) {
  header {
    .container {
      #menu {
        .connect {
          margin-left: 0;
        }
        .menu {
          li {
            a {
              color: var(--white-two);
              font-size: 15px;
              font-family: "Work Sans", sans-serif;
            }
          }
        }
      }
      .content {
        .left {
          .two-bt {
            margin-left: 25px;
          }
        }
        .right {
          margin-left: 5%;
        }
      }
    }
  }
}

@media (max-width: 1170px) {
  /* br {
    display: none;
  } */
  span {
    br {
      display: none;
    }
  }
  header {
    .effect-banner {
      width: 70%;
      height: 871px;
      margin-top: 830px;
      margin-right: 150px;
    }
    .container {
      #menu {
        .menu {
          margin-left: 365px;
        }
      }
      .content {
        padding-top: 60px;
        flex-direction: column;
        display: flex;
        align-items: center;
        .title {
          font-size: 85px;
          text-align: center;
        }
        .one-bt {
          font-size: 28px;
          margin-left: 100px;
        }
        .two-bt {
          font-size: 28px;
        }
        .numbers {
          margin-left: 95px;
          .one {
            h1 {
              font-size: 44px;
            }
            p {
              font-size: 20px;
              padding-left: 31px;
            }
          }
          .two {
            h1 {
              font-size: 44px;
            }
            p {
              font-size: 20px;
              padding-left: 31px;
            }
          }
          .three {
            h1 {
              font-size: 44px;
            }
            p {
              font-size: 20px;
              padding-left: 31px;
            }
          }
        }
        .right {
          .banner {
            margin-top: 100px;
            .timer {
              width: 512px;
              height: 90px;
            }
          }
        }
      }
    }
  }
}

@media (max-width: 1100px) {
  header {
    & .container {
      & #menu {
        .menu {
          margin-left: 300px;
        }
      }
    }
  }
}

@media (max-width: 1000px) {
  header {
    & .container {
      & #menu {
        .menu {
          margin-left: 200px;
        }
      }
      & .content {
        .numbers {
          margin-left: 40px;
        }
        .one-bt {
          margin-left: 50px;
        }
        .left {
          margin-left: 0;
          .title {
            font-size: 75px;
          }
        }
      }
    }
  }
}

@media (max-width: 900px) {
  header {
    & .container {
      #menu {
        .menu {
          margin-left: 100px;
        }
      }
      & .content {
        & .left {
          .title {
            font-size: 65px;
          }
        }
        .one-bt {
          margin-left: 0;
        }
        .numbers {
          margin-left: 0;
        }
        .right {
          .banner {
            margin-top: 160px;
          }
        }
      }
    }
  }
}

@media (max-width: 800px) {
  .body_wraper {
    overflow: hidden;
    visibility: visible;
  }
  .menu-icon {
    display: block;
    position: absolute;
    right: 0;
    top: 55px;
    margin-right: 80px;
    cursor: pointer;
    /* z-index: -1; */
  }
  .menu-icon {
    display: block;
  }
  header {
    & .container {
      & #menu {
        .menu {
          position: absolute;
          top: 0;
          right: -364px;
          width: 320px;
          height: 100%;
          background: #251928;
          margin-left: 450px;
          flex-direction: column;
          padding-top: 60px;
          z-index: 10;
          transition: 0.5s;

          li {
            padding-top: 25px;
            margin-top: 20px;
            padding-bottom: 12px;
            margin-left: auto;
            margin-right: auto;
            a {
              font-size: 25px;
            }
          }
        }
        .menu:focus > .menu {
          visibility: visible;
        }
        .connect {
          display: none;
          font-size: 20px;
          margin-top: 582px;
        }
      }
    }
  }
  .burger-checkbox {
    position: absolute;
    visibility: hidden;
  }
  .burger {
    z-index: 11;
    cursor: pointer;
    display: block;
    position: relative;
    border: none;
    background: transparent;
    width: 40px;
    height: 26px;
    margin-top: 20px;
    margin-left: auto;
    margin-right: 80px;
  }
  .burger::before,
  .burger::after {
    content: "";
    left: 0;
    position: absolute;
    display: block;
    width: 100%;
    height: 4px;
    border-radius: 10px;
    background: #ffce4e;
  }
  .burger::before {
    top: 0;
    box-shadow: 0 11px 0 #ffce4e;
    transition: box-shadow 0.3s 0.15s, top 0.3s 0.15s, transform 0.3s;
  }
  .burger::after {
    bottom: 0;
    transition: bottom 0.3s 0.15s, transform 0.3s;
  }
  .burger-checkbox:checked + .burger::before {
    top: 11px;
    transform: rotate(45deg);
    box-shadow: 0 6px 0 rgba(0, 0, 0, 0);
    transition: box-shadow 0.15s, top 0.3s, transform 0.3s 0.15s;
  }
  .burger-checkbox:checked + .burger::after {
    bottom: 11px;
    transform: rotate(-45deg);
    transition: bottom 0.3s, transform 0.3s 0.15s;
  }
  .burger-checkbox:checked ~ .menu {
    transform: translateX(-300px);
  }
}

@media (max-width: 768px) {
  header {
    padding-bottom: 150px;
    .effect-banner {
      display: none;
    }
    .container {
      & .content {
        & .right {
          .banner {
            display: none;
            width: 90%;
            .timer {
              margin-left: 10px;
              width: 400px;
              .current-bid {
                h1 {
                  margin-top: 7px;
                  font-family: "Oxanium", sans-serif;
                  font-weight: 700;
                  font-size: 26px;
                  color: #fff;
                }
              }
              .ends {
                margin-left: 142px;
              }
            }
            .user {
              width: 490px;
              button {
                margin-left: 70px;
              }
              .artist {
                margin-left: 50px;
              }
            }
          }
        }
      }
    }
  }
}

@media (max-width: 600px) {
  header {
    & .container {
      & .content {
        .one-bt {
          font-size: 20px;
          margin-left: 15px;
        }
        .two-bt {
          font-size: 20px;
        }
        .numbers {
          .one {
            h1 {
              font-size: 40px;
            }
          }
          .two {
            margin-left: 30px;
            h1 {
              font-size: 40px;
            }
          }
          .three {
            margin-left: 30px;
            h1 {
              font-size: 40px;
            }
          }
        }
        & .left {
          .title {
            font-size: 55px;
          }
        }
      }
    }
  }
}

@media (max-width: 500px) {
  header {
    & .container {
      & .content {
        .one-bt {
          font-size: 20px;
          padding: 24px 56px;
        }
        .two-bt {
          font-size: 20px;
          padding: 24px 56px;
        }
        .left {
          .title {
            font-size: 45px;
          }
        }
        .numbers {
          .one {
            h1 {
              font-size: 30px;
              margin-left: 35px;
            }
            p {
              padding-left: 25px;
            }
          }
          .two {
            h1 {
              font-size: 30px;
              margin-left: 25px;
            }
            p {
              padding-left: 15px;
            }
          }
          .three {
            h1 {
              font-size: 30px;
              margin-left: 25px;
            }
            p {
              padding-left: 15px;
            }
          }
        }
      }
    }
  }
}

@media (max-width: 425px) {
  header {
    & .container {
      & .content {
        .left {
          .title {
            font-size: 40px;
          }
        }
        .one-bt {
          font-size: 20px;
          padding: 20px 46px;
        }
        .two-bt {
          font-size: 20px;
          padding: 20px 46px;
        }
      }
    }
  }
}
</style>
