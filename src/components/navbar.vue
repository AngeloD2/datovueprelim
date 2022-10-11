<template>

  <div className="navBar">
    <div className="logo"> <img src="../assets/sbit.png"> </div>
  <div className="btn-container">
     <button className="btn-home" onclick="window.location.href='#home'"> Home </button> 
      <button className="btn-skills" onclick="window.location.href='#skills'"> Skills </button> 
      <button className="btn-portfolio" onclick="window.location.href='#portfolio'"> Portfolio </button> 
      <button className="btn-contact" onclick="window.location.href='#contact'"> Contact Me </button> 
    </div>
  </div>

</template>

<script>

  export default {
    name: 'NavBar'
  }
  </script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
template {
  display:flex;
  flex-direction:row;
}
.navBar {
  position:fixed;
  display:flex;
  flex-direction:row;
  justify-content:space-around;
  width:100%;
  max-width:65em;
  height:3em;
  background-color:whitesmoke;
  border-radius:1em;
  margin-top:-5.5em;
}
.logo, .logo img{
  height:3em;
}
.logo {
  width:2em;
  display:flex;
  justify-content:flex-start;
  margin-left:1em;
}
.btn-container {
  display:flex;
  width:100%;
  justify-content:flex-end;
  align-self:end;
  gap:2em;
  margin-right:2em;
}

.btn-container a:hover, .btn-home:hover, .btn-skills:hover, .btn-portfolio:hover, .btn-contact:hover {
  border-radius:0.3em;
  background-color:rgb(209, 209, 209);
}
.btn-home, .btn-skills, .btn-portfolio, .btn-contact {
  display:flex;
  text-decoration:none;
  align-self:center;
  color:black;
  border:none;
  font-weight:100;
  font-size:medium;
  line-height:1;
  padding:1.2em 1em;
  background-color:whitesmoke;
}
a {
  display:flex;
  text-decoration:none;
  align-self:center;
  color:white;
  border:none;
  font-weight:100;
  font-size:medium;
}

@media screen and (max-width: 850px) {

.navBar {
  position:fixed;
  display:flex;
  flex-direction:row;
  justify-content:space-around;
  width:100%;
  max-width:65em;
  height:3em;
  background-color:whitesmoke;
  border-radius:1em;
  margin-top:-5.3em;
}

a {
  background-color:none;
}
.btn-home, .btn-skills, .btn-portfolio, .btn-contact { 
  background-color:none;
  height:3em;
  align-content:center;
}
}
</style>
