<template>
  <div className="container">

    <div class="content">
      <div className="hi"> 
        <div className="hiText">
        <h1> Interested? </h1>
        <p> Contact me through these channels: </p>
        <div className="trad"> 
        <p> Mobile: {{mobile}}</p>
        <p> Landline: {{landline}}</p>
        <p> E-Mail: {{email}}</p>
      </div>
        </div>
      <div className="image"> <img src="../assets/contactimg.png">  </div>
      </div>

      <div className="sMedia">
        <h3> Connect through my socials: </h3>
        <div class="icons"> 
          <div className="fb"> <img src="../assets/fb.png"> <p> /angelo.dato.92 </p> </div>
          <div className="insta"> <img src="../assets/insta.png"> /inigo.d2 </div>
        </div>
      </div>

      <div className="revisit">
       <div> <h4> Return to: </h4> </div> 
        <div className="btn-container">
     <button className="btn" onclick="window.location.href='#home'"> Home </button> 
      <button className="btn" onclick="window.location.href='#skills'"> Skills </button> 
      <button className="btn" onclick="window.location.href='#portfolio'"> Portfolio </button> 
      <button className="btn" onclick="window.location.href='#contact'"> Contact </button> 
    </div>
    </div>
    </div>

  </div>
</template>

<script>


export default {
  name: 'contacT',
  props: {
    mobile: Number,
    landline: Number,
    email: String,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

a {
  color: #42b983;
}
.content {
  display:flex;
  flex-wrap:wrap;
  width:100%;
  gap:2em;
}
.hi {
  display:flex;
  width:100%;
  justify-content:space-around;
  
}
.hiText {
  display:flex;
  flex-direction:column;
  width:35%;
  background-color:rgb(224, 224, 224);
  border-radius:1em 1em 1em 5em;
  margin-top:1em;
  color:black;
}
.hiText h1, .hiText p {
  display:flex;
  align-self:center;
}
.image {
  display:flex;
  width:50%;
  justify-content:end;
  height:45rem;
  border:1em hidden;
  border-radius:1em 5em 1em 5em;
  margin-top:1em;
  background-color:rgb(224, 224, 224);
  /*background: -webkit-linear-gradient(gold, purple,aqua, gold );*/
}
.image img{
  margin-top:-1em;
}
.trad {
  display:flex;
  flex-direction:column;
}
.trad p{
  align-self:flex-start;
  margin-left:1em;
}
.sMedia {
  color:black;
  margin-top:3em;
  margin-left:2em;
  display:flex;
  flex-direction:column;
  border-radius:1em;
  background-color:rgb(224, 224, 224);
  width:35%;
}
.sMedia h3 {
  display:flex;
  margin-left:1em;
}
.icons {
  display:flex;
  flex-direction:column;
}
.icons img {
  height:2.5em;
}
.fb, .insta {
  display:flex;
  flex-direction:row;
  width:90%;
  gap:2em;
  justify-content:flex-start;
  margin-left:1em;
}
.revisit {
  color:black;
  margin-top:3em;
  margin-left:2.5em;
  display:flex;
  flex-direction:column;
  border-radius:1em;
  background-color:rgb(224, 224, 224);
  width:50%;
}
.btn-container {
  display:flex;
  flex-direction:row;
  gap:1em;
  justify-content:center;
}
.btn {
  display:flex;
  border:none;
  font-weight:bold;
  color:black;
  font-size:1em;
  border:0.1em transparent whitesmoke;
  padding-left:1.4em;
  padding-right:1.4em;
  padding-top:1em;
  padding-bottom:1em;
  background: -webkit-linear-gradient(gold, purple);
  border-radius:25em 1em 25em 1em;
  align-self:center;
}

@media screen and (max-width: 850px) {

.container {
  display:flex;
  justify-content:space-around;
}
.content {
  display:flex;
  flex-direction:row;
  flex-wrap:wrap;
  justify-content:flex-start;
  gap:5em;
}
.hi {
  display:flex;
  width:100%;
  flex-wrap:wrap;
}
.hiText {
  font-size:0.58em;
  padding:0;
  height:fit-content;
  width:35%;
}
.trad p{
  align-self:flex-start;
  margin-left:3em;
}
.sMedia {
  font-size:0.65em;
  margin:0;
  margin-top:-10em;
  margin-left:2em;
}
.image img {
  border-radius:1em 5em 1em 5em;
}
.image {
  height:fit-content;
}
.revisit {
  color:black;
  margin-top:3em;
  margin-left:2.5em;
  display:flex;
  flex-direction:column;
  border-radius:1em;
  background-color:rgb(224, 224, 224);
  width:100%;
}
.btn {
  display:flex;
  border:none;
  font-weight:bold;
  color:black;
  font-size:1em;
  border:0.1em transparent whitesmoke;
  padding:1em;
  background: -webkit-linear-gradient(gold, purple);
  border-radius:25em 1em 25em 1em;
  align-self:center;
}
}
</style>
