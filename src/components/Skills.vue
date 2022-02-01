<template>
<section id="Skills">
  <!-- <br><br><br> -->
  <div class="myskills">My Skills</div>
    <div class="skillscontainer">
    <div class="bar front advanced" data-skill="HTML"></div>
    <div class="bar back advanced" data-skill="CSS"></div>
    <div class="bar back basic" data-skill="Javascript"></div>
    <div class="bar front advanced" data-skill="Bootstrap"></div>
    <div class="bar front expert" data-skill="Vue"></div>
  </div>
  </section>
</template>

<script>
export default {

}
</script>

<style>
 #Skills {
   padding-top: 100px;
    background-color:  rgb(95, 93, 93);
    background-size: cover;
    background-repeat: no-repeat;
    height: 100vh;
  }
  .skillscontainer {
     /* float: right; */
      width: 65% !important;
      margin-right: auto;
      margin-left: auto;
      margin-top: 200px;
  }
  
  .myskills {
       justify-content: center;
       font-weight: 50px;
       font-size: 50px;
       color: white;

  }


  .s-h1 {
    text-align: center;
  }

  body{
  font-family: Helvetica, Arial, sans-serif;
}
.container{
  width: 50%;
  margin: 0 auto;
}
@keyframes load{
  from {
    width: 0%
  }
}
@-webkit-keyframes load{
  from {
    width: 0%
  }
}
@-moz-keyframes load{
  from {
    width: 0%
  }
}
@-o-keyframes load{
  from {
    width: 0%
  }
}

.bar{
  background-color: #EEE;
  padding: 2px;
  border-radius: 15px;
  margin-bottom: 5px;
  font-size: 14px;
  color: #FFF;
  font-weight: bold;
  text-shadow: 1px 1px 1px rgba(0,0,0,0.5);
}
.bar::before{
  content:  attr(data-skill);
  background-color: #f3b0ff;
  display: inline-block;
  padding: 5px 0 5px 10px;
  border-radius: inherit;
  animation: load 2s 0s;
  -webkit-animation: load 2s 0s;
  -moz-animation: load 2s 0s;
  -o-animation: load 2s 0s;
}

.bar.front::before{
  background-color: #ffcc33;
}
.bar.back::before{
  background-color: #a6cfe3;
}

.bar.learning::before{
  width: calc(20% - 10px);
}
.bar.basic::before{
  width: calc(40% - 10px);
}
.bar.intermediate::before{
  width: calc(60% - 10px);
}
.bar.advanced::before{
  width: calc(80% - 10px);
}
.bar.expert::before{
  width: calc(100% - 10px);
}

</style>