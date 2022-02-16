<template>
  <div class="container">
    <HeaderView />

    <div class="menu-content">
      <div class="saudation">
        <h1>{{ msg }}</h1>
        <small>{{ subMsg }}</small>
      </div>

      <div class="row justify-content-end">
        <div class="col-lg-4 col-md-6 col-sm-12">
          <div class="box">
            <span>04</span>
            <p>Warriors ready to protect Cardania</p>
          </div>
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12">
          <div class="box">
            <span>58</span>
            <p>CwP obtained with the claim of your warriors</p>
          </div>
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12">
          <div class="box">
            <span>01</span>
            <p>Island that is being prepared for you</p>
          </div>
        </div>
      </div>

      <div class="row justify-content-end">
        <div class="col-md-6 col-sm-12">
          <div class="box2">
            <div>
              <i class="bi bi-check-circle"></i>
              <span> Wallet Connected</span>
            </div>
            <div>
              <span class="alert">{{ wallet }}</span>
            </div>
          </div>
        </div>
        <div class="col-md-6 col-sm-12">
          <div class="box2">
            <div>
              <i class="bi bi-exclamation-circle"></i>
              <span> Two-factor authentication not enabled</span>
            </div>
            <div>
              <span class="alert">{{ enabled }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="mt-5">
      <MenuLateral />
    </div>
  </div>
</template>

<script>
import HeaderView from "./HeaderView.vue";
import MenuLateral from "./MenuLateral.vue";
export default {
  name: "BaseComponentes",
  components: {
    HeaderView,
    MenuLateral,
  },
  data() {
    return {
      msg: "Hi, Warrior!",
      subMsg: "This is a little about you..",
      wallet: "WALLET",
      enabled: "ENABLE",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  text-decoration: none;
  color: #d5d5d565;
}
.saudation {
  text-align: initial;
  margin-bottom: 20px;
}
.menu-content {
  flex-direction: column;
  display: flex;
  width: 70%;
  float: right;
}
.box {
  background: rgba(0, 0, 0, 0.486);
  height: 100px;
  display: flex;
  padding: 20px;
  border-radius: 10px;
  margin-top: 20px;
  align-items: center;
}
.box > span {
  font-size: 48px;
  font-weight: 600px;
}
.box2 {
  background: rgba(255, 255, 255, 0.082);
  display: flex;
  padding: 20px;
  margin-top: 20px;
  border-radius: 10px;
  justify-content: space-between;
  align-items: center;
  color: #fff;
  align-items: center;
}
.box2 .alert {
  padding: 10px;
  background: #00000085;
}
@media (max-width: 768px) {
  .MenuLateral,
  .MenuLateral2 {
    display: none;
  }
  .menu-content {
    width: 100%;
  }
}
</style>
