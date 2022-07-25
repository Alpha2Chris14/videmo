<template>
  <header>
    <nav class="header">
      <div class="logo">
          <h1>VIDEMO</h1>
        </div>
      <ul class="nav_item" ref="navItem">
        <li><a href="#">Home</a></li>
        <li><a href="#">Trending</a></li>
        <li><a href="#">Categories</a></li>
        <li><a href="#">Featured</a></li>
        <li><a href="#" id="sign">Sign In</a></li>
      </ul>

      <div class="mobileMenu" v-on:click = "toogle">
        <div></div>
        <div></div>
        <div></div>
      </div>
    </nav>
  </header>
</template>

<style scoped>
header{
  background-blend-mode: darken;
  background-image: url("../assets/bg.png");
  background-position-y: -200px;
  height: 100vh;
}
.header {
  display: flex;
  background: rgb(16, 15, 15, 0.8);
  align-items: center;
  color: rgb(242, 170, 37);
  height: 10vh;
  padding-left: 2vw;
  padding-right: 2vw;
  z-index: 2;
  position: fixed;
  width: 100vw;
}

.logo {
  flex-grow: 2;
}

.nav_item {
  display: flex;
  list-style: none;
  justify-content: space-around;
  flex-grow: 2;
}

li {
  width: 100%;
  text-align: center;
}

.nav_item a {
  text-decoration: none;
  color: rgb(255, 166, 0);
  transition: font-size;
  transition-duration: 0.2s;
  transition-timing-function: linear;
}

.nav_item a:hover {
  text-decoration: none;
  color: rgb(255, 166, 0);
  border-bottom: 2px solid rgb(255, 166, 0);
  border-width: 2px;
  font-size: 18px;
}

.mobileMenu{
  display: none;
}

#sign {
  border: 2px solid rgb(255, 166, 0);
  border-radius: 5px;
  padding: 10px;
  color: rgb(255, 166, 0);
  font-weight: bold;
  background: rgb(16, 15, 15, 0.8);
  transition: all;
  transition-duration: 0.5s;
}

#sign:hover {
  border: 2px solid rgb(255, 166, 0);
  border-radius: 5px;
  padding: 10px;
  color: rgb(16, 15, 15, 0.8);
  background: rgb(255, 166, 0);
  font-weight: bolder;
}
@media screen and (max-width:750px) {
  header{
  background-position-y: -300px;
  height: 70vh;
  max-height: 100vh;
}
}
@media screen and (max-width:800px) {
  .nav_item{
    position: absolute;
    display: flex;
    flex-direction: column;
    right:  0px;
    top:74px;
    background: rgb(16, 15, 15, 0.8);
    border-top: 1px solid rgb(29, 28, 28);
    height: 100vh;
    width: 40vw;
    transition: all;
    transition-duration: 0.8s;
    transition-delay: 0.1s;
    transform: translateX(40vw);
    padding-bottom: 20vh;
  }
  .mobileMenu{
    display: block;
  }

  .mobileMenu div{
    width: 35px;
    height: 6px;
    background: rgb(255, 166, 0);
    margin:4px;
  }
}
</style>

<script>
export default {
  data() {
    return {
      open:false,
    }
  },

  methods: {
    toogle:function(){
      let nav = this.$refs.navItem;
      this.open = !this.open;
      console.log(this.open);
      if(this.open == true){
        nav.style.transform = "translateX(0vw)";
      }else{
        
        nav.style.transform = "translateX(40vw)";
      }
    },
  },
};
</script>