<template>
  <div class="header">
    <div class="nav">
      <div class="topbar">
        <div class="logo">
          <img src="@/assets/img/logo_ras.jpg" alt="" />
          <h3>broome.art</h3>
        </div>
        <div class="aside">
          <p>Upload</p>
          <p>Contacts</p>
          <p>Login</p>
        </div>
      </div>
      <div class="article">
        <p>Лучшие интерьерные картины с высококачественной печатью HD.</p>
        <input type="text" placeholder="Search for paintings" />
      </div>
    </div>
  </div>
</template>

<script></script>

<style lang="less" scoped>
.header {
  background: url(@/assets/img/main_bg2.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background-position-y: -90px;
  height: 500px;
  position: relative;

  &::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.4);
    top: 0;
    left: 0;
    z-index: 0;
  }

  .nav {
    max-width: 1600px;
    padding: 0 30px;
    margin: auto;
    .topbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 80px;
      position: relative;

      .logo {
        display: flex;
        align-items: center;
        img {
          height: 50px;
          width: 50px;
          border-radius: 50%;
          margin-right: 8px;
        }
        h3 {
          color: #fff;
          font-size: 24px;
        }
      }
      .aside {
        display: flex;
        align-items: center;
        p {
          color: #fff;
          margin-left: 30px;
          font-size: 18px;
          font-weight: 500;
        }
      }
    }
    .article {
      display: flex;
      align-self: center;
      position: relative;
      width: 100%;
      max-width: 630px;
      margin: auto;
      padding-top: 100px;
      flex-wrap: wrap;
      p {
        font-size: 34px;
        color: #fff;
        line-height: 40px;
        letter-spacing: -0.2px;
        font-weight: 500;
      }
      input {
        width: 550px;
        font-size: 18px;
        padding: 15px 4px 15px 20px;
        border-radius: 10px;
        color: #1d1d1d;
        margin-top: 30px;
      }
    }
  }
}
</style>
