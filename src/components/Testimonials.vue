<template>
<section id="Testimonials">
  <br><br><br>
<div class="main">
  <div class="testhead">Testimonials</div>
  <ul class="cards">
    <li class="cards_item">
      <div class="card">
        <div class="card_image"><img src="https://media.discordapp.net/attachments/898466432864645152/898466764671827968/me2.jpg?width=478&height=300"></div>
        <div class="card_content">
          <h2 class="card_title">Leigh-Anne</h2>
          <p class="card_text">Aspiring Front-End Developer</p>
          <p class="card_text">Craig is very focused when it comes to his work especially the visual parts. He is a real creative!      
            <br>
            <br>
          </p>
        </div>
      </div>
    </li>
    <li class="cards_item">
      <div class="card">
        <div class="card_image"><img src="https://media.discordapp.net/attachments/897834164357836820/897850338495852544/20210922_104043.jpg?width=478&height=300"></div>
        <div class="card_content">
          <h2 class="card_title">Zharne</h2>
          <p class="card_text">Aspiring Front-End Developer</p>
          <p class="card_text">Craig is really always willing to listen to you. Remembers what you tell him and always gives his
            best.</p>
        </div>
      </div>
    </li>
    <li class="cards_item">
      <div class="card">
        <div class="card_image"><img src="https://media.discordapp.net/attachments/897462426793050122/897812760904224798/Screenshot_20211013_134204.jpg?width=478&height=300"></div>
        <div class="card_content">
          <h2 class="card_title">Tursha</h2>
          <p class="card_text">Aspiring Front-End Developer</p>
          <p class="card_text">Craig is a extremely vibrant person. He always ensure that he's work is polished and looking good. </p>
        </div>
      </div>
    </li>
    <li class="cards_item">
      <div class="card">
        <div class="card_image"><img src="https://media.discordapp.net/attachments/895010077080182795/897428091285155850/MG_5341.JPG?width=478&height=300"></div>
        <div class="card_content">
          <h2 class="card_title">Enosh</h2>
          <p class="card_text">Aspiring Front-End Developer</p>
          <p class="card_text">Craig is a very compassionate and uncomplicated person.<br>
             He does exceptionally well with styling and decorating his web pages.</p>
        </div>
      </div>
    </li>
    <li class="cards_item">
      <div class="card">
        <div class="card_image"><img src="https://media.discordapp.net/attachments/898505129924395009/898530137925091358/me.jpg?width=478&height=300"></div>
        <div class="card_content">
          <h2 class="card_title">Tony</h2>
          <p class="card_text">Aspiring Front-End Developer</p>
          <p class="card_text">Craig is a very influencial person with remarkable enthusiams and with the most resfreshing energy.<br><br></p>
        </div>
      </div>
    </li>
    <li class="cards_item">
      <div class="card">
        <div class="card_image"><img src="https://media.discordapp.net/attachments/895009723445817425/903598546811514951/1625390188691.jpg?width=478&height=300"></div>
        <div class="card_content">
          <h2 class="card_title">Alex</h2>
          <p class="card_text">Lecturer</p>
          <p class="card_text">Craig is a creative and mindful individual. He always brings life in the room and takes pride in his work.<br><br></p>
        </div>
      </div>
    </li>
  </ul>
</div>
  </section>
</template>

<script>
export default {

}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Quicksand:400,700');

#Testimonials {
   background-color: rgb(95, 93, 93);
    background-size: cover;
    background-repeat: no-repeat;
    height: 100vh;
}

.main{
  max-width: 1200px;
  margin: 0 auto;
}

.testhead {
    font-size: 50px;
    font-weight: 400;
    text-align: center;
    color: white;
}

img {
  height: auto;
  max-width: 100%;
  vertical-align: middle;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  list-style: none;
  margin: 0;
  padding: 0;
}

.cards_item {
  display: flex;
  padding: 1rem;
}

@media (min-width: 40rem) {
  .cards_item {
    width: 50%;
  }
}

@media (min-width: 56rem) {
  .cards_item {
    width: 33.3333%;
  }
}

.card {
  background-color: white;
  border-radius: 0.25rem;
  box-shadow: 0 20px 40px -14px rgba(0, 0, 0, 0.25);
  display: flex;
  flex-direction: column;
  overflow: hidden;
}

.card_content {
  padding: 1rem;
  background: linear-gradient(to bottom left, #ffffff 10%, #ffffff 100%);
}

.card_title {
  color: #000000;
  font-size: 1.1rem;
  font-weight: 700;
  letter-spacing: 1px;
  text-transform: capitalize;
  margin: 0px;
}

.card_text {
  color: #000000;
  font-size: 0.875rem;
  line-height: 1.5;
  margin-bottom: 1.25rem;    
  font-weight: 400;
}
.made_by{
  font-weight: 400;
  font-size: 13px;
  margin-top: 35px;
  text-align: center;
}
</style>