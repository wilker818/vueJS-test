<template>
  <ul class="MenuLateral">
    <li>
      <a href=""> <i class="bi bi-wallet"></i><span> Wallet</span> </a>
    </li>
    <li>
      <a href="">
        <i class="bi bi-arrow-left-right"></i>
        <span> Claim</span>
      </a>
    </li>
    <li>
      <a href="">
        <i class="bi bi-shield-check"></i>
        <span> Security</span>
      </a>
    </li>
    <li>
      <a href="">
        <i class="bi bi-person-circle"></i>
        <span> Profile</span>
      </a>
    </li>
  </ul>

  <ul class="MenuLateral2">
    <li>
      <small>External Links</small>
    </li>
    <li>
      <span> Island Editor</span>
      <i class="bi bi-box-arrow-in-up-right"></i>
    </li>
    <li>
      <span> Index</span>
      <i class="bi bi-box-arrow-in-up-right"></i>
    </li>
  </ul>
</template>
<script>
export default {
  name: "MenuLateral",
  data() {
    return {};
  },
};
</script>

<style scoped>
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
.MenuLateral {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  flex-wrap: nowrap;
  width: 30%;
}
.MenuLateral > li {
  margin-bottom: 10px;
  font-size: 30px;
  font-weight: 700px;
  color: #d5d5d565;
}
.MenuLateral2 {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  flex-wrap: nowrap;
  width: 30%;
}
.MenuLateral2 li > small {
  font-size: 16px;
  color: #d5d5d565;
}
.MenuLateral2 > li {
  margin-bottom: 10px;
  font-size: 30px;
  font-weight: 700px;
  color: #fff;
}

@media (max-width: 768px) {
  .MenuLateral2{
    display: none;
  }
  .MenuLateral{
    display: none;
  }
}
</style>
