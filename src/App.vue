<template>
  <div class="container">
  <section id="1" style="background-color: red">
    <div class="choice">
      <div class="question">ARE YOU FRANK ZAPPA?</div>
      <a href="#2">YES</a>
      <a href="#">NO</a>
    </div>
  </section>

  <section id="2" style="background-color: black">
    <div class="choice">
      <div class="question">ARE YOU FRANK ZAPPA?</div>
      <a href="">YES</a>
      <a href="">NO</a>
    </div>
  </section>

  <section style="background-color: yellow">
    <div class="choice">
      <div class="question">ARE YOU FRANK ZAPPA?</div>
      <a href="">YES</a>
      <a href="">NO</a>
    </div>
  </section>

  <section style="background-color: green">
    <div class="choice">
      <div class="question">ARE YOU FRANK ZAPPA?</div>
      <a href="">YES</a>
      <a href="">NO</a>
    </div>
  </section>

  </div>
</template>

<script>

export default {};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Zen+Tokyo+Zoo&display=swap');
*{
  box-sizing: border-box;
}
html{}
body {
  margin: 0;
  padding: 0;
}
section{
  height: 100vh;
  width: 100%;
  display: flex;

}
.choice{
  width: 50%;
  margin: auto;
  text-align: center;
  padding: 40px;
  border: 3px solid white;
}

.question{
  color: white;
  font-size: 50px;
  font-family: "Zen Tokyo Zoo", cursive;
  margin-bottom: 20px;
}

.choice a  {
  color: black;
  font-size: 20px;
  padding-right: 20px;
  font-family: "Zen Tokyo Zoo",serif;
  background-color: whitesmoke;
  margin: 5px;
  text-align: center;
  padding: 10px;
  text-decoration: none;
  border-radius: 4px;

}
</style>