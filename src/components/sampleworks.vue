<template>
  <div class="container">
    <div class="head">  </div>

    <div class="content">
      <div class="port">
        <div className="jobName"> 
          <div class="jobTitle"> <h4> Hotel Management App</h4> </div>  
          <div class="jobDesc"> <p> Made with React.JS</p> </div>  
        </div> 
        <div className="image2"> 
          <img src="../assets/react.jpg"> 
          <img src="../assets/react2.jpg">
          <img src="../assets/react3.jpg">
        </div>
        
      </div>

      <div class="port">
        <div className="jobName"> 
          <div class="jobTitle"> <h4> Point of Sale App </h4> </div>  
          <div class="jobDesc"> <p> Made with HTML / PHP / SQL </p> </div>  
        </div> 
          
        <div className="image2"> 
          <img src="../assets/pos.jpg"> 
          <img src="../assets/pos2.jpg">
        </div>
                
      </div>
      <div class="port">
        <div className="jobName"> 
          <div class="jobTitle"> <h4> Portfolio Website </h4> </div>  
          <div class="jobDesc">  <p> Mockup made with HTML / CSS</p> </div>  
        </div> 
        <div className="image2"> 
          <img src="../assets/mockup.jpg"> 
          <img src="../assets/mockup2.jpg">
        </div>
      </div>

      <div class="port">
        <div className="jobName2"> 
          <div class="jobTitle2"> <h4> - Art on the Side - </h4> </div>  
        </div> 
        <div class="imgContainer">
              <div class="image"> <img src="../assets/1.jpg"> </div>
              <div class="image"> <img src="../assets/2.jpg"> </div>
              <div class="image"> <img src="../assets/3.jpg"> </div>
              <div class="image"> <img src="../assets/4.png"> </div>
        </div>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
  name: 'PortFolio',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

a {
  color: #42b983;
}

.head {
  height:2em;
}
.content {
  display:flex;
  flex-direction:column;
  width:100%;
}
.port {
  display:flex;
  flex-direction:column;
  justify-content:center;
  width:100%;
  
}

.jobName, .jobName2 {
  display:flex;
  flex-direction:row;
  border-radius:5em 5em 1em 1em;
  justify-content:space-around;
  color:black;
}

.jobName2 {
  border-radius:1em 1em 0em 0em;
  width:100%;
}
.jobTitle2 {
  display:flex;
  justify-content:space-around;
  width:25%;
  background-color:purple;
  color:white;
  border-radius:1em;
  margin-bottom:0.5em;
}
.jobName h4, .jobName h3{
  display:flex;
  justify-self:end;
  flex-direction:row;
}

.jobTitle, .jobDesc {
  display:flex;
  justify-content:space-around;
  width:25%;
  background-color:rgb(224, 224, 224);
  border-radius:1em;
}

.jobDesc {
  background-color: purple;
}
.jobDesc p{
  align-self:center;
  font-size:0.8em;
  color:white;
}

.image {
  display:flex;
  height:25em;
  
}
.image2 {
  display:flex;
  margin-top:1rem;
  margin-bottom:1em;
  flex-direction:row;
  justify-content:space-evenly;
  flex-wrap: wrap;
  background:-webkit-linear-gradient(whitesmoke,rgb(223, 222, 222),whitesmoke);
  border-radius:0.4em;
}
.image2 img{
  display:flex;
  width:100%;
  margin-top:1rem;
  margin-bottom:1em;
  max-width:25em;
  border-radius:0.5em;
  transition:0.15s ease;
  border:0.3em solid rgb(224, 224, 224);
}
img:hover{
  transform:scale(1.05);
}

.imgContainer {
  display:flex;
  flex-direction: row;
  transition:0.15s ease;
  border:0.3em solid rgb(224, 224, 224);
  padding:1em;
}
.imgContainer img {
  display:flex;
  flex-direction: row;
  width:95%;
  border-radius:1em;
  transition:0.15s ease;
}

@media screen and (max-width: 850px) {

.container {
  display:flex;

}
.content {
  display:flex;
  gap:5em;
}
h4 {
  font-size:0.8em;
}
.jobDesc {
  font-size:0.65em;
}
.imgContainer {
  display:flex;
  flex-direction:row;
  gap:1em;
}
.port {
  height:fit-content;
}
.imgContainer img {
  height:15em;
  width:10em;
}
.image {
  height:fit-content;
}
}

</style>
