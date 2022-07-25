<template>
  <section class="newletterContainer">
    <h2>Subscribe To Our News Letter</h2>
    <p>Be the first to know when something amazing comes up-just subscribe</p>
    <div class="formArea">
      <input type="email" name="" id="" />
      <input type="submit" value="SUBSCRIBE" />
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.newletterContainer {
  background-color: whitesmoke;
  height: max-content;
  text-align: center;
  padding-top: 50px;
  padding-left: 10vw;
  padding-right: 10vw;
  padding-bottom: 50px;
}

.newletterContainer h2 {
  font-weight: bold;
  font-size: 2.5rem;
  margin-bottom: 25px;
}

p {
  font-size: 1.6rem;
  padding-left: 10vw;
  padding-right: 10vw;
}

.formArea {
  display: flex;
  padding-top: 40px;
  padding-left: 20vw;
  padding-right: 20vw;
}

input{
    padding:8px
}

input[type="email"]{    
    width: 250%;
    outline: none;
    border:1px groove grey;
    border-right: none;
}


input[type="submit"]{    
    width: 100%;
    background-color:rgb(242, 170, 37);
    border: none;
    color: white;
    font-size: 20px;
    border-top-right-radius: 10px;
    border-bottom-right-radius: 10px;
}

input[type="submit"]:hover{
    cursor: pointer;
}

@media screen and (max-width:650px) {
  .formArea{
    padding-left: 1vw;
    padding-right: 1vw;
    flex-direction: column;
  }

  input[type="email"]{    
    width: 100%;
    border-right: 1px solid grey;
}

input[type="submit"]{    
    border-top-right-radius: 0px;
    border-bottom-right-radius: 0px;
    margin-top: 1vh;
}
}
</style>