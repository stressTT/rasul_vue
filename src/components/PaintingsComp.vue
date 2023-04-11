<template>
  <div class="main">
    <div class="nav">
      <p @click="myFilter()" v-bind:class="{ active: isActive }">Popular</p>
      <p>New</p>
      <p>Special</p>
    </div>
    <h4>Интерьерные картины</h4>
    <div class="article">
      <div class="first">
        <img src="@/assets/img/img1.jpg" alt="" />
        <img src="@/assets/img/img2.jpg" alt="" />
        <img src="@/assets/img/img3.jpg" alt="" />
        <img src="@/assets/img/img4.jpg" alt="" />
        <img src="@/assets/img/img5.jpg" alt="" />
        <img src="@/assets/img/img6.jpg" alt="" />
      </div>
      <div class="second">
        <img src="@/assets/img/img6.jpg" alt="" />
        <img src="@/assets/img/img1.jpg" alt="" />
        <img src="@/assets/img/img4.jpg" alt="" />
        <img src="@/assets/img/img3.jpg" alt="" />
        <img src="@/assets/img/img5.jpg" alt="" />
        <img src="@/assets/img/img2.jpg" alt="" />
      </div>
      <div class="third">
        <img src="@/assets/img/img5.jpg" alt="" />
        <img src="@/assets/img/img6.jpg" alt="" />
        <img src="@/assets/img/img1.jpg" alt="" />
        <img src="@/assets/img/img3.jpg" alt="" />
        <img src="@/assets/img/img2.jpg" alt="" />
        <img src="@/assets/img/img4.jpg" alt="" />
      </div>
    </div>
  </div>
</template>

<style lang="less" scoped>
.main {
  max-width: 1600px;
  padding: 0 30px;
  margin: 30px auto;

  .nav {
    display: flex;
    margin: auto;
    justify-content: center;
    margin-bottom: 30px;
    p {
      padding: 15px 20px;
      font-size: 16px;
      transition: all 0.3ms;
      cursor: pointer;
    }
    .active {
      background: #000;
      color: #fff;
      margin: 0 10px;
      border-radius: 24px;
    }
  }
  h4 {
    font-size: 24px;
    font-weight: 500;
    letter-spacing: -0.2px;
  }
  .article {
    margin-top: 30px;
    display: flex;
    flex-wrap: wrap;
    width: 100%;
    justify-content: space-between;
    div {
      width: 520px;

      img {
        width: 520px;
        object-fit: contain;
        align-self: flex-start;
        height: fit-content;

        margin-bottom: 16px;
      }
    }
  }
}
</style>

<script>
export default {
  data() {
    return {
      isActive: true,
    };
  },
  methods: {
    myFilter: function () {
      console.log("123");
      this.isActive = !this.isActive;
      // some code to filter users
    },
  },
};
</script>
