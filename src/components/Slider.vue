<template>
  <div class="banner_section">
    <div class="overlay"></div>
    <div class="content_container">
      <h2>Hi Welcome To Videmo,</h2>
      <h2>Unlimited Shows, And More.</h2>
      <p>Home To Everything Entertainment</p>
      <a href="#" class="btn">GET STARTED</a>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.banner_section{
    width: 100vw;
}
.overlay {
  background-color: black;
  height: 100vh;
  opacity: 0.7;
  position: absolute;
  width: 100vw;
  top: 0;
}

.content_container {
  margin-top: 35vh;
  top: 0;
  position: absolute;
  padding-left: 20px;
}

h2 {
  color: white;
  font-size: 3.8rem;
}
h2:nth-child(2) {
  font-size: 3rem;
}
p {
  color: rgb(255, 182, 48);
  font-size: 2rem;
  margin-top: 0.6rem;
  margin-bottom: 1.8rem;
}

.btn {
  background-color: rgb(255, 182, 48);
  text-decoration: none;
  color: white;
  font-size: 1.5rem;
  padding: 1vw;
  font-weight: bold;
  transition: all;
  transition-duration: 0.4s;
  /* box-shadow: 0 10px 12px 12px rgb(9, 6, 6); */
}

.btn:hover {
  border-radius: 10px;
  border: 2px solid rgb(255, 166, 0);
  background: rgb(16, 15, 15, 0.8);
  color: rgb(255, 166, 0);
}

@media screen and (max-width:740px) {
  .content_container {
  margin-top: 25vh;
}

  h2 {
  color: white;
  font-size: 2.5rem;
}
h2:nth-child(2) {
  font-size: 2rem;
}
p {
  
  font-size: 1.2rem;
}

.btn {
  font-size: 1rem;
  border-radius: 10px;
  padding: 10px;
}
}

@media screen and (max-width:750px) {
  .overlay{

  height: 70vh;
  max-height: 100vh;
}
}
</style>