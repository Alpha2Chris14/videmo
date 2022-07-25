<template>
  <section>
    <div class="spacer"></div>
    <div class="left_content">
      <img src="../assets/kid.png" alt="kid" srcset="" />
    </div>
    <div class="right_content">
      <h2>Create profiles for kids.</h2>
      <p>
        Send kids on adventures with their favorite characters in a space made
        just for them—free with your membership
      </p>
    </div>
    <div class="spacer"></div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
section {
  background: black;
  color: white;
  display: flex;
  width: 100%;
  justify-content: space-around;
}

.spacer {
  flex-grow: 2;
  width: 20%;
}
img {
  width: 500px;
  height: 400px;
}

.right_content {
  align-self: center;
}

.right_content h2 {
  font-weight: bold;
  font-size: 2.5rem;
  margin-bottom: 10px;
}

p {
  font-size: 1.2rem;
  text-transform: lowercase;
}

@media screen and (max-width: 650px) {
  img {
    width: 35vw;
    height: 30vh;
  }
}

@media screen and (max-width: 500px) {
  section{
    flex-direction: column;
    padding: 2vw 10vh;
    align-items: center;
    text-align: center;
  }

  img {
    width: 100vw;
    height: 50vh;
  }
}
</style>