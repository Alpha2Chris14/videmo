<template>
  <footer>
    <section class="footer">
      <div class="left">
        <a href="">ABOUT</a>
        <a href="">POLICY</a>
        <a href="">TERMS OF SERVICE</a>
        <a href="">CONTACT</a>
      </div>
      <div class="spacer" id="space"></div>
      <div class="right">
        <img src="../assets/logo_facebook.svg" alt="" srcset="" />
        <img src="../assets/logo_instagram.svg" alt="" srcset="" />
        <img src="../assets/logo_twitter.svg" alt="" srcset="" />
      </div>
    </section>
    <div class="divider">
      <hr />
    </div>
    <div class="app">
      <div class="spacer"></div>
      <img src="../assets/google.svg" alt="playstore" srcset="" />
      <img src="../assets/ios.svg" alt="applestore" srcset="" />
      <div class="spacer"></div>
    </div>
    <div class="copy">
      <p>Copyright &copy; 2020 Videmo. inc</p>
      <p>
        Videmo is a registered trademark of Videmo, Inc. All rights reserved.
      </p>
      <p>Made with &hearts; Chris</p>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped>
footer {
  background-color: black;
  color: white;
  display: flex;
  padding: 3vh 2vw;
  flex-direction: column;
}
.footer {
  display: flex;
  margin-top: 20px;
}

p {
  font-size: 10px;
  color: rgb(242, 170, 37);
}
a {
  text-decoration: none;
  color: rgb(242, 170, 37);
  font-size: 1rem;
}

a:hover {
  color: white;
}
.spacer {
  flex-grow: 2;
  width: 100%;
}
.left {
  display: flex;
  justify-content: space-evenly;
  width: 100%;
}

.right {
  display: flex;
  justify-content: space-evenly;
  width: 30%;
}
img {
  width: 15px;
}
img:hover {
  cursor: pointer;
}

.divider {
  padding-left: 2vw;
  padding-right: 2vw;
}
hr {
  border: 1px solid rgba(138, 137, 136, 0.8);
  margin-top: 20px;
}
.app {
  display: flex;
  align-content: space-evenly;
}
.app img {
  height: 150px;
  width: 150px;
  margin-left: 1vw;
}

.copy {
  text-align: center;
}

.copy p {
  font-size: 0.9rem;
}

@media screen and (max-width: 650px) {
  #space {
    display:none;
  }
}
@media screen and (max-width: 700px) {
  .spacer {
    flex-grow: 1;
  }
}
@media screen and (max-width: 894px) {
  .left a {
    font-size: 0.7rem;
  }
}
</style>                  j            