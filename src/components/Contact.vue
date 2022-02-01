<template>

  <section id="Contact">
    <br><br><br>  
<body>
  <div class="contacthead">Get In Touch!</div>
  <div class="contactcontainer">
    <div class="content">
      <div class="left-side">
        <div class="address details">
          <i class="fas fa-map-marker-alt"></i>
          <div class="topic">Address</div>
          <div class="text-one">3 Queens Drive, Colorado Park</div>
          <div class="text-two">Mitchells Plain</div>
        </div>
        <div class="phone details">
          <i class="fas fa-phone-alt"></i>
          <div class="topic">Phone</div>
          <div class="text-one">0685680287</div>
        </div>
        <div class="email details">
          <i class="fas fa-envelope"></i>
          <div class="topic">Email</div>
          <div class="text-one">braafcraig@gmail.com</div>
        </div>
      </div>
      <div class="right-side">
        <div class="topic-text">Send us a message</div>
        <div class="contactpara">If you have any work for me or queries related to my work, you can send me message from here. It's my pleasure to help you.</div>
      <form method ="POST" action="https://formspree.io/f/mvodyone"> 
        <div class="input-box">
          <input type="text" name="name" placeholder="Enter your name" required>
        </div>
        <div class="input-box">
          <input type="text" name="email" placeholder="Enter your email" required>
        </div>
        <div class="input-box message-box">
          <input type="text" name="message" placeholder="Enter Message">
        </div>
        <div class="button">
          <input type="submit" value="Send Now" >
        </div>
      </form>
    </div>
    </div>
  </div>
</body>
</section>
</template>

<script>
export default {

}
</script>

<style>
 #Contact {
    background-color:  rgb(95, 93, 93);
    background-size: cover;
    background-repeat: no-repeat;
    height: 100vh;
  }

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');
*{
  font-family: "Poppins" , sans-serif;
}

body{
  padding-top: 85px;
  width: 100%;
  align-items: center;
  justify-content: center;
}

.contacthead {
  color: white;
  justify-content: center;
  font-weight: 50px;
  font-size: 50px;
  
}

.contactcontainer{
  margin-top: 100px;
  margin-left: auto;
  margin-right: auto;
  width: 55%;
  background: #fff;
  border-radius: 6px;
  padding: 20px 60px 30px 40px;
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  height: 500px;
}
.contactcontainer .content{
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.container .content .left-side{
  width: 25%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin-top: 15px;
  position: relative;
}
.content .left-side::before{
  content: '';
  position: absolute;
  height: 70%;
  width: 2px;
  right: -15px;
  top: 50%;
  transform: translateY(-50%);
  background: #afafb6;
}
.content .left-side .details{
  margin: 14px;
  text-align: center;
}
.content .left-side .details i{
  font-size: 30px;
  color: #000000;
  margin-bottom: 10px;
}
.content .left-side .details .topic{
  font-size: 18px;
  font-weight: 500;
}
.content .left-side .details .text-one,
.content .left-side .details .text-two{
  font-size: 14px;
  color: #afafb6;
}
.contactcontainer .content .right-side{
  width: 75%;
  margin-left: 75px;
}
.content .right-side .topic-text{
  font-size: 23px;
  font-weight: 600;
  color:  #000000;
}
.right-side .input-box{
  height: 50px;
  width: 100%;
  margin: 12px 0;
}
.right-side .input-box input,
.right-side .input-box textarea{
  height: 100%;
  width: 100%;
  border: none;
  outline: none;
  font-size: 16px;
  background: #F0F1F8;
  border-radius: 6px;
  padding: 0 15px;
  resize: none;
}
.right-side .message-box{
  min-height: 110px;
}
.right-side .input-box textarea{
  padding-top: 6px;
}
.right-side .button{
  display: inline-block;
  margin-top: 12px;
}
.right-side .button input[type="button"]{
  color: #fff;
  font-size: 18px;
  outline: none;
  border: none;
  padding: 8px 16px;
  border-radius: 6px;
  background:  #505050;
  cursor: pointer;
  transition: all 0.3s ease;
}
.button input[type="button"]:hover{
  background:  #000000;
}

@media (max-width: 950px) {
  .contactcontainer{
    width: 90%;
    padding: 30px 40px 40px 35px ;
  }
  .contactcontainer .content .right-side{
   width: 75%;
   margin-left: 55px;
}
}
@media (max-width: 820px) {
  .contactcontainer{
    margin: 40px 0;
    height: 100%;
  }
  .contactcontainer .content{
    flex-direction: column-reverse;
  }
 .contactcontainer .content .left-side{
   width: 100%;
   flex-direction: row;
   margin-top: 40px;
   justify-content: center;
   flex-wrap: wrap;
 }
 .contactcontainer .content .left-side::before{
   display: none;
 }
 .contactcontainer .content .right-side{
   width: 100%;
   margin-left: 0;
 }
}

.contactpara {
  font-size: 15px;
}
</style>