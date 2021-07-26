<template>
  <div class="container">
  <section v-for="choice in choices"
           :key="choice.id"
           :id="choice.id"
           :style="{'background-color':choice.background}">
    <div class="choice">
      <div class="question">{{choice.question}}</div>
      <a v-for="link in choice.links"
         :key="link"
         :href="link.href"
         :style="{ color:choice.background }" >
         {{ link.label }}

      </a>
    </div>
  </section>

  </div>
</template>

<script>

export default {
  data(){
    return{
      choices:[
        {
          id: 1,
          question: "Are you the best guitarist ever?",
          links: [
            {href: "#3", label: "Yes" },
            {href: "#5", label: "No" },
          ],
          background: "#1B264F"
        },
        {
          id: 2,
          question: "Do you have the coolest mustache?",
          links: [
            {href: "#4", label: "Yes" },
            {href: "#5", label: "No" },
          ],
          background: "#FF5F45"
        },{
          id: 3,
          question: "Girl, you thought he was a man, But he was a muffin?",
          links: [
            {href: "#2", label: "Yes" },
            {href: "#5", label: "No" },
          ],
          background: "#D98324"
        },{
          id: 4,
          question: "Moving to Montana soon?",
          links: [
            {href: "#6", label: "Yes" },
            {href: "#5", label: "No" },
          ],
          background: "#A40606"
        },{
          id: 5,
          question: "So... you are not Frank Zappa",
          links: [
            {href: "#1", label: "Nope...." },
          ],
          background: "#D7CF07"
        },{
          id: 6,
          question: "Then You Are FRANK ZAPPA",
          links: [
            {href: "https://www.youtube.com/watch?v=_q0nImsfMvE", label: "HELL YES" },
          ],
          background: "#230007"
        },
      ]
    }
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Zen+Tokyo+Zoo&display=swap');
*{
  box-sizing: border-box;
}
html{
  scroll-behavior: smooth;
}
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