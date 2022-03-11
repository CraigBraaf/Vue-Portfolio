<template>
 
    <section id="About">
    <br><br><br>
    <div class="aboutcontainer">
    <div id="left"> <img src="https://media.discordapp.net/attachments/931437059778945056/937370577252024352/IMG-20220130-WA0007.jpg">
    </div>


    <div id="right">
    <div class="aboutheading">ABOUT ME</div>
    <div class="whycoding">Why Coding?</div>
    <div class="para">Techology has always striked my interest as a child and just developed into something I really love spending time with. Im also really creative with visuals and coding makes a perfect path career path, considering it allows me to be creative on a visual level with technological platforms like visual code.</div><br>
    <div class="details">
      <b>Name</b>: Craig
      <br>
      <b>Surname</b>: Braaf
      <br>
      <b>Contact</b>: 0685680287
      <br>
      <b>Email</b>: Braafcraig@gmail.com
     <br>
      <div class="details2">
        <b>Age</b>: 22<br>
        <b>From</b>: Cape Town, SA
      </div>

       <div class="sub-main">
      <a target="_blank" href="https://docs.google.com/document/d/15Br488WIhKmaVbRHkUn0LTEGfADeHF0c/edit"><button class="button-three">Download CV</button></a>
    </div>

      <div class="icons"><div class="wrapper">
  <a target="_blank" href="https://codepen.io/CraigBraaf">
    <div class="icon codepen">
      <div class="tooltip">
        Codepen
      </div>
      <span><i class="fab fa-codepen"></i></span>
    </div>
  </a>
  <a target="_blank" href="https://github.com/CraigBraaf">
    <div class="icon github">
      <div class="tooltip">
        Github
      </div>
      <span><i class="fab fa-github"></i></span>
    </div>
  </a>
  <a target="_blank" href="https://www.linkedin.com/in/craig-braaf-b47769224/">
    <div class="icon linkedin">
      <div class="tooltip">
        LinkedIn
      </div>
      <span><i class="fab fa-linkedin"></i></span>
    </div>
  </a>
</div></div>
    </div>
    </div>
    </div>
    </section>
   

</template>

<script>
export default {

}
</script>

<style scoped>

 #About {
    background-color:  rgb(95, 93, 93);
    background-size: cover;
    background-repeat: no-repeat;
    height: 100vh;
  }

.aboutheading{
  color: rgb(32, 32, 32);
  font-weight: 900;
  font-size: 90px !important;
  padding-top: 60px;
}

.whycoding {
    font-weight: 900;
    font-size: 30px !important;
}

#right{
    float: right;
    width: 600px;
    height: 800px;
    color: rgb(0, 0, 0);
    align-items: flex-start;
    margin-top: 10px;
    margin-right: 200px;
    border: 0px 10pxblack;
}

#left {
   float: left;
   width: 600px;
   height: 800px;
   border-radius: 20px;
   margin-top: 80px;
   margin-left: 150px;
   
}

img {
  height: 100% !important;
  border-radius: 10px;
}

.aboutcontainer {
  background: white ;
  /* border-radius: 20px; */
  margin-left: 150px;
  height: 90%;
  width: 85%;
  margin-right: 100px;



}

.details {
  text-align: initial;
}

.details2 {
  float: right;
  margin-top: -103px;
  justify-content: initial;
}

.icons {
  margin-top: 60px;
  margin-left: 150px;
}

a {
  color: #222;
}
.wrapper {
  display: inline-flex;
}
.wrapper .icon {
  margin: 0 20px;
  text-align: center;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  position: relative;
  z-index: 2;
  transition: 0.4s cubic-bezier(0.68, -0.55, 0.265, 1.55);
}
.wrapper .icon span {
  display: block;
  height: 60px;
  width: 60px;
  background: #fff;
  border-radius: 50%;
  position: relative;
  z-index: 2;
  box-shadow: 0px 10px 10px rgba(0, 0, 0, 0.1);
  transition: 0.4s cubic-bezier(0.68, -0.55, 0.265, 1.55);
}
.wrapper .icon span i {
  line-height: 60px;
  font-size: 25px;
}
.wrapper .icon .tooltip {
  position: absolute;
  top: 0;
  z-index: 1;
  background: #fff;
  color: #fff;
  padding: 10px 18px;
  font-size: 20px;
  font-weight: 500;
  border-radius: 25px;
  opacity: 0;
  pointer-events: none;
  box-shadow: 0px 10px 10px rgba(0, 0, 0, 0.1);
  transition: 0.4s cubic-bezier(0.68, -0.55, 0.265, 1.55);
}
.wrapper .icon:hover .tooltip {
  top: -70px;
  opacity: 1;
  pointer-events: auto;
}
.icon .tooltip:before {
  position: absolute;
  content: "";
  height: 15px;
  width: 15px;
  background: #fff;
  left: 50%;
  bottom: -6px;
  transform: translateX(-50%) rotate(45deg);
  transition: 0.4s cubic-bezier(0.68, -0.55, 0.265, 1.55);
}
.wrapper .icon:hover span {
  color: #fff;
}
.wrapper .icon:hover span,
.wrapper .icon:hover .tooltip {
  text-shadow: 0px -1px 0px rgba(0, 0, 0, 0.4);
}
.wrapper .codepen:hover span,
.wrapper .codepen:hover .tooltip,
.wrapper .codepen:hover .tooltip:before {
  background: #000000;
}
.wrapper .github:hover span,
.wrapper .github:hover .tooltip,
.wrapper .github:hover .tooltip:before {
  background: #333;
}
.wrapper .linkedin:hover span,
.wrapper .linkedin:hover .tooltip,
.wrapper .linkedin:hover .tooltip:before {
  background: #0033db;
}


.button-three {
    position: relative;
    background-color: #b6b6b6;
    border: none;
    padding: 20px;
    width: 200px;
    text-align: center;
    -webkit-transition-duration: 0.4s; /* Safari */
    transition-duration: 0.4s;
    text-decoration: none;
    overflow: hidden;
}

.button-three:hover{
   background:#fff;
   box-shadow:0px 2px 10px 5px #97B1BF;
   color:#000;
}

.button-three:after {
    content: "";
    background: #f1c40f;
    display: block;
    position: absolute;
    padding-top: 300%;
    padding-left: 350%;
    margin-left: -20px !important;
    margin-top: -120%;
    opacity: 0;
    transition: all 0.8s
}

.button-three:active:after {
    padding: 0;
    margin: 0;
    opacity: 1;
    transition: 0s
}

.sub-main {
  margin-left: 210px;
  padding-top: 150px;
}
</style>