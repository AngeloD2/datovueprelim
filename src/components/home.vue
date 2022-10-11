<template>
  <div className="container">

    <div className="description">
      <div>  <h3 className="greet"> {{greetings}} </h3> </div>
      <div>  <h1 className="name"> {{name}} </h1></div>
      <div>  <p className="title"> {{title}} </p></div>
      <div>  <p className="desc"> {{desc}} </p></div>

      <button className="call" onclick="window.location.href='#skills'"> Let's go! </button>
    </div>
    <div className="imageContainer">  <img src="../assets/owo3.png"> </div>
  </div>
</template>

<script>
export default {
  name: 'homE',
  props: {
    greetings:String,
    name: String,
    title:String,
    desc:String,
    img:Image
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  display:flex;
  margin-top:5em;
}
.img, .imageContainer{
  border-radius:5em;
  height:25em;
  width:fit-content;
}
.imageContainer {
  display:flex;
  width:25%;
  /*background: -webkit-linear-gradient(gold, purple,aqua, gold, white );*/
  background-color:rgb(255, 213, 140);
  box-shadow: rgb(212, 212, 212);
  border:1em transparent;
  border-radius:1em 20em 1em 25em;
  justify-content:flex-end;
  overflow:hidden; 
}
img {
  display:flex;
  justify-self:flex-end;
  height:25em;
}
.description {
  display:flex;
  flex-direction: column;
  justify-content:center;
  align-self:center;
  width:35%;
  height:100%;
}
.greet, .name{
  display:flex;
  color:darkslategrey;
}
.greet {
  margin-bottom:-0.5em;
  font-size:2em;
}
.name {
  height:1.2em;
  font-size:3em;
}
.title{ 
  display:flex;
  margin-top:-1em;
  box-shadow:0em 0.3em gold;
  font-size:1em;
  color:grey;
}
.desc {
  display:flex;
  align-self:flex-start;
  width:100%;
  max-width:23em;
  font-size:0.8em;
  color:rgb(20, 20, 20);
}
.call {
  display:flex;
  border:none;
  font-weight:bold;
  color:black;
  font-size:x-large;
  border:0.1em transparent whitesmoke;
  background: -webkit-linear-gradient(gold, purple);
  border-radius:25em 1em 25em 1em;
  padding-left:3.2em;
  padding-right:3.2em;
  padding-bottom:0.5em;
  padding-top:0.5em;
  margin-top:4em;
  align-self:center;

}
@media screen and (max-width: 850px) {

  .container {
    display:flex;
    flex-direction:row;
    gap:5em;
  }
  .imageContainer, .description {
    display:flex;
  }
  .title {
    margin-top:2em;
  }
}


</style>
