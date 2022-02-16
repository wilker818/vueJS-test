<template>
  <header>
    <ul class="HeaderMenu">
      <li>
        <img
          src="https://pbs.twimg.com/profile_banners/1379607294372110337/1633284987/1500x500"
          alt="CardanoWarriors"          
        />
      </li>    

      <li>
        <div id="menu-hamburguer" class="btn-group">
          <a class="bi bi-list"  id="dropdownMenuClickableOutside" data-bs-toggle="dropdown" data-bs-auto-close="inside" aria-expanded="false">            
          </a>
          <ul class="dropdown-menu" aria-labelledby="dropdownMenuClickableOutside">            
              <li>
                <a class="dropdown-item" href="/wallet">
                  <span> Wallet</span>
                </a>
              </li>
              <li>
                <a class="dropdown-item" href="/claim">                  
                  <span> Claim</span>
                </a>
              </li>
              <li>
                <a class="dropdown-item" href="/security">                  
                  <span> Security</span>
                </a>
              </li>
              <li>
                <a class="dropdown-item" href="/profile">                 
                  <span> Profile</span>
                </a>
              </li> 
              <li>
                <small class="dropdown-item">External Links</small>
              </li>
              <li>
                <a class="dropdown-item" href="/island-editor">
                  <span> Island Editor</span>  
                </a>             
              </li>
              <li>
                <a class="dropdown-item" href="/">
                <span> Index</span>
                </a>                
              </li>
          </ul>
        </div>

        <a href="/logout" id="logOut">
          <span>Log out </span>
          <i class="bi bi-arrow-bar-right"></i>
        </a>
      </li>
    </ul>
  </header>
</template>
<script>
export default {
  name: "HeaderView",
  components: {},
  data() {
    return {};
  },
};
</script>

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
}
.HeaderMenu {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
}
.HeaderMenu img {
  width: 200px;
  height: 80px;
}


@media (max-width: 768px) {
  #menu-hamburguer {
    display: block !important;
  }
  #menu-hamburguer a {
    font-size: 40px;
  }
  #logOut {
    display: none;
  }
  #menu-hamburguer .MenuLateral > li {
    color: #000;
  }
  #menu-hamburguer .MenuLateral2 > li {
    color: #000;
  }
}
#menu-hamburguer {
  display: none;
}
</style>
