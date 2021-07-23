<template>
  <section style="background-color: red">
    <div class="choice">
      <div class="question">ARE YOU ROB STARK?</div>
      <a href="">YES</a>
      <a href="">NO</a>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
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
}
</style>