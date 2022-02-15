<template>
  <div class="container">

    <header>
      <ul class="HeaderMenu">
        <li>
          <img src="https://pbs.twimg.com/profile_banners/1379607294372110337/1633284987/1500x500" alt="CardanoWarriors" width="200px" height="100px">
        </li>

        <li>
          <a href="">
            <span> Log out</span>
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-bar-right" viewBox="0 0 16 16">
              <path fill-rule="evenodd" d="M6 8a.5.5 0 0 0 .5.5h5.793l-2.147 2.146a.5.5 0 0 0 .708.708l3-3a.5.5 0 0 0 0-.708l-3-3a.5.5 0 0 0-.708.708L12.293 7.5H6.5A.5.5 0 0 0 6 8zm-2.5 7a.5.5 0 0 1-.5-.5v-13a.5.5 0 0 1 1 0v13a.5.5 0 0 1-.5.5z"/>
            </svg>
          </a>
        </li>
      </ul>
    </header>

    <div class="menu-content">
      <div class="saudation">  
        <h1>{{ msg }}</h1>
        <small>{{ subMsg }}</small>
      </div>
      
      <div class="row justify-content-end">       
        <div class="col-sm-4">
          <div class="box"> 
            <span>04</span>
            <p>Warriors ready to protect Cardania</p>
          </div>
        </div>
        <div class="col-sm-4" >
          <div class="box">
            <span>58</span>
            <p>CwP obtained with the claim of your warriors</p>
          </div>
        </div>
        <div class="col-sm-4" >
          <div class="box">
            <span>01</span>
            <p>Island that is being prepared for you</p>
          </div>
        </div>
      </div>

      <div class="row justify-content-end">       
        <div class="col-sm-6">
          <div class="box2"> 
            <div>
              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-circle" viewBox="0 0 16 16">
                <path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/>
                <path d="M10.97 4.97a.235.235 0 0 0-.02.022L7.477 9.417 5.384 7.323a.75.75 0 0 0-1.06 1.06L6.97 11.03a.75.75 0 0 0 1.079-.02l3.992-4.99a.75.75 0 0 0-1.071-1.05z"/>
              </svg>
              <span>Wallet Connected</span>
            </div>
            <div>
              <span class="alert">{{ wallet }}</span>
            </div>
          </div>
        </div>
        <div class="col-sm-6" >
          <div class="box2">
            <div>
              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-exclamation-circle" viewBox="0 0 16 16">
                <path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/>
                <path d="M7.002 11a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 4.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 4.995z"/>
              </svg>
              <span>Two-factor authentication not enabled</span>
            </div>
            <div>
              <span class="alert">{{ enabled }}</span>
            </div>
          </div>
        </div>        
      </div>

    </div>
  <div>
    <ul class="MenuLateral">
      <li>
        <a href="">
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-wallet2" viewBox="0 0 16 16">
            <path d="M12.136.326A1.5 1.5 0 0 1 14 1.78V3h.5A1.5 1.5 0 0 1 16 4.5v9a1.5 1.5 0 0 1-1.5 1.5h-13A1.5 1.5 0 0 1 0 13.5v-9a1.5 1.5 0 0 1 1.432-1.499L12.136.326zM5.562 3H13V1.78a.5.5 0 0 0-.621-.484L5.562 3zM1.5 4a.5.5 0 0 0-.5.5v9a.5.5 0 0 0 .5.5h13a.5.5 0 0 0 .5-.5v-9a.5.5 0 0 0-.5-.5h-13z"/>
          </svg><i class="bi bi-wallet"></i><span> Wallet</span>
        </a>  
      </li>
      <li>
        <a href=""> 
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-left-right" viewBox="0 0 16 16">
            <path fill-rule="evenodd" d="M1 11.5a.5.5 0 0 0 .5.5h11.793l-3.147 3.146a.5.5 0 0 0 .708.708l4-4a.5.5 0 0 0 0-.708l-4-4a.5.5 0 0 0-.708.708L13.293 11H1.5a.5.5 0 0 0-.5.5zm14-7a.5.5 0 0 1-.5.5H2.707l3.147 3.146a.5.5 0 1 1-.708.708l-4-4a.5.5 0 0 1 0-.708l4-4a.5.5 0 1 1 .708.708L2.707 4H14.5a.5.5 0 0 1 .5.5z"/>
          </svg><span> Claim</span>
        </a>
      </li>
      <li>
        <a href="">
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-shield-check" viewBox="0 0 16 16">
            <path d="M5.338 1.59a61.44 61.44 0 0 0-2.837.856.481.481 0 0 0-.328.39c-.554 4.157.726 7.19 2.253 9.188a10.725 10.725 0 0 0 2.287 2.233c.346.244.652.42.893.533.12.057.218.095.293.118a.55.55 0 0 0 .101.025.615.615 0 0 0 .1-.025c.076-.023.174-.061.294-.118.24-.113.547-.29.893-.533a10.726 10.726 0 0 0 2.287-2.233c1.527-1.997 2.807-5.031 2.253-9.188a.48.48 0 0 0-.328-.39c-.651-.213-1.75-.56-2.837-.855C9.552 1.29 8.531 1.067 8 1.067c-.53 0-1.552.223-2.662.524zM5.072.56C6.157.265 7.31 0 8 0s1.843.265 2.928.56c1.11.3 2.229.655 2.887.87a1.54 1.54 0 0 1 1.044 1.262c.596 4.477-.787 7.795-2.465 9.99a11.775 11.775 0 0 1-2.517 2.453 7.159 7.159 0 0 1-1.048.625c-.28.132-.581.24-.829.24s-.548-.108-.829-.24a7.158 7.158 0 0 1-1.048-.625 11.777 11.777 0 0 1-2.517-2.453C1.928 10.487.545 7.169 1.141 2.692A1.54 1.54 0 0 1 2.185 1.43 62.456 62.456 0 0 1 5.072.56z"/>
            <path d="M10.854 5.146a.5.5 0 0 1 0 .708l-3 3a.5.5 0 0 1-.708 0l-1.5-1.5a.5.5 0 1 1 .708-.708L7.5 7.793l2.646-2.647a.5.5 0 0 1 .708 0z"/>
          </svg><span> Security</span>
        </a>
      </li>
      <li>
        <a href="">
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-person-circle" viewBox="0 0 16 16">
            <path d="M11 6a3 3 0 1 1-6 0 3 3 0 0 1 6 0z"/>
            <path fill-rule="evenodd" d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8zm8-7a7 7 0 0 0-5.468 11.37C3.242 11.226 4.805 10 8 10s4.757 1.225 5.468 2.37A7 7 0 0 0 8 1z"/>
          </svg><span> Profile</span>
        </a>
      </li>
    </ul>      
  </div>
  <ul class="MenuLateral2">
      <li>
        <small>External Links</small>
      </li>
      <li>
        <span> Island Editor</span>
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-in-up-right" viewBox="0 0 16 16">
          <path fill-rule="evenodd" d="M6.364 13.5a.5.5 0 0 0 .5.5H13.5a1.5 1.5 0 0 0 1.5-1.5v-10A1.5 1.5 0 0 0 13.5 1h-10A1.5 1.5 0 0 0 2 2.5v6.636a.5.5 0 1 0 1 0V2.5a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 .5.5v10a.5.5 0 0 1-.5.5H6.864a.5.5 0 0 0-.5.5z"/>
          <path fill-rule="evenodd" d="M11 5.5a.5.5 0 0 0-.5-.5h-5a.5.5 0 0 0 0 1h3.793l-8.147 8.146a.5.5 0 0 0 .708.708L10 6.707V10.5a.5.5 0 0 0 1 0v-5z"/>
        </svg> 
      </li>
      <li>
        <span> Index</span>
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-in-up-right" viewBox="0 0 16 16">
          <path fill-rule="evenodd" d="M6.364 13.5a.5.5 0 0 0 .5.5H13.5a1.5 1.5 0 0 0 1.5-1.5v-10A1.5 1.5 0 0 0 13.5 1h-10A1.5 1.5 0 0 0 2 2.5v6.636a.5.5 0 1 0 1 0V2.5a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 .5.5v10a.5.5 0 0 1-.5.5H6.864a.5.5 0 0 0-.5.5z"/>
          <path fill-rule="evenodd" d="M11 5.5a.5.5 0 0 0-.5-.5h-5a.5.5 0 0 0 0 1h3.793l-8.147 8.146a.5.5 0 0 0 .708.708L10 6.707V10.5a.5.5 0 0 0 1 0v-5z"/>
        </svg>
      </li>      
    </ul>      
  </div>


</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Hi, Warrior!',
      subMsg: 'This is a little about you..',
      wallet: 'WALLET',
      enabled: 'ENABLE',
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
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
.saudation{
  text-align: initial;
  margin-bottom: 20px;
}
.HeaderMenu{
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.menu-content{
  flex-direction: column;
  display: flex;
  width: 70%;
  float: right;

}
.MenuLateral{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  flex-wrap: nowrap;
  width: 30%;
  
}
.MenuLateral>li{
  margin-bottom: 10px;
  font-size: 30px;
  font-weight: 700px;
  color: #d5d5d565;
}
.MenuLateral2{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  flex-wrap: nowrap;
  width: 30%;
  
}
.MenuLateral2 li > small{
  font-size: 16px;
  color: #d5d5d565;
}
.MenuLateral2>li{
  margin-bottom: 10px;
  font-size: 30px;
  font-weight: 700px;
  color: #fff;
}
.box{  
  background: rgba(0, 0, 0, 0.301);  
  height: 100px;
  display: flex;
  padding: 20px;
  border-radius: 10px;

}
.box > span{
  font-size: 48px;
  font-weight: 600px;
}
.box2{  
  background: rgba(255, 255, 255, 0.082);  
  display: flex;
  padding: 20px;
  margin-top: 20px;
  border-radius: 10px;
  justify-content: space-between;
  align-items: center;

}
.box2 .alert{
  padding: 10px;
  background: #00000085;
}
</style>
