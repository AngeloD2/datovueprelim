<template>
  <div class="container">
    <div class="content">

      <div class="skill">
        <div class="imageContainer"> <img src="../assets/html.png"> </div>
        <p> Accustomed to all HTML-5 tags for the past 6 years, <br/>
            building an HTML website is like second nature.</p>
            
      <h1> HTML </h1>
      </div>

      
      <div class="skill2">
        <div class="imageContainer"> <img src="../assets/css.png"> </div>
        <p> HTML is all but bland without CSS. <br/>
            Bring your ideas to life with CSS Grid and Flex.</p>

      <h1> CSS </h1>
      </div>

      <div class="skill">
        <div class="imageContainer"> <img src="../assets/reactLogo.png"> </div>
        <p> Interactive websites with minimal reloading <br/> while working with dynamic content.</p>
      <h1> REACT </h1>
      </div>

      <div class="skill2">
        <div class="imageContainer"> <img src="../assets/phpLogo.png"> </div>
        <p> A scripting language and is similar to HTML. <br/>
            PHP is able to handle more dynamic content.</p>
      <h1> PHP </h1>
      </div>
    </div>
</div>

</template>

<script>
export default {
  name: 'SkillS',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.container {
  justify-content:space-around;
}

.content {
  display:flex;
  flex-direction:column;
  flex-wrap:wrap;
  width:100%;
}

p {
  display:flex;
  width:100%;
  max-width:25em;
  color:black;
  font-size:1.6rem;
  height:fit-content;
  align-self:center;
  padding-top:1.5em;
  padding-bottom:1.5em;
  border-radius:1em;
}
.content :nth-child(2n+0) {
  display:flex;
  width:100%;
  flex-direction:row-reverse;
  
  
}
.imageContainer2{
  display:flex;
  width:100%;
  max-width:28rem;
  flex-direction:row-reverse;
  background-color:rgb(224, 224, 224);
  
}

.imageContainer, .imageContainer img{
  display:flex;
  width:100%;
  max-width:28rem;
  border-radius:1em;
}
.skill {
  display:flex;
  flex-direction:row;
  justify-content:space-around;
  border-top:0.5em hidden;
  margin-top:1em;

}
.skill2 {
  display:flex;
  margin-top:3em;
  justify-content:space-around;
  padding-top:3em;
  padding-bottom:3em;
  flex-direction:row-reverse;
  background:-webkit-linear-gradient(whitesmoke,rgb(206, 206, 206),whitesmoke )
}

.skill h1, .skill2 h1{
  display:flex;
  color:white;
  height:fit-content;
  width:100%;
  max-width:5em;
  background-color:purple;
  border-radius:1em 5em 5em 1em;
  padding:0.5em;
  align-self:center;
  transition:0.15s ease;
}
.skill h1:hover, .skill2 h1:hover{
  transform:scale(1.1);
  text-decoration:none;
}
.skill h1 {
  border-radius:5em 1em 1em 5em;
}

@media screen and (max-width: 850px) {

.container {
  display:flex;

}
.content {
  display:flex;
  flex-direction:row;
  gap:5em;
}
.title {
  margin-top:2em;
}
}

</style>
