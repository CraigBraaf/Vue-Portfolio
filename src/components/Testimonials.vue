<template>
<section id="Testimonials">
  <br><br><br>
<div class="main">
  <div class="testhead">Testimonials</div>
  <div v-for="testimonial in testimonials" :key="testimonial" class="card">
    <div  class="cards_item">
      <div   class="card">
        <div class="card_image"><img :src="testimonial.img"></div>
        <div class="card_content">
          <h2 class="card_title">{{testimonial.name}}</h2>
          <p class="card_text">{{testimonial.position}}</p>
          <p class="card_text">{{testimonial.description}}      
            <br>
            <br>
          </p>
        </div>
      </div>
    </div>
  </div>
  
</div>
  </section>
</template>



<script>

const url = "https://craigbraaf-api.herokuapp.com/"
export default {
  data(){
    return {
      testimonials:[]
    };
  },
   
  mounted(){
    fetch(`${url}testimonials`)
    .then((res) => res.json())
    .then(data => this.testimonials = data)
    .catch(err => console.log(err.message))
  }}

</script>

<style scoped>
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
  margin-top: -200px;
}

.testhead {
    font-size: 50px;
    font-weight: 400;
    text-align: center;
    color: white;
}

img {
  max-width: 100%;
  vertical-align: middle;
  object-fit: cover;
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
  justify-content: center;
  align-content: center;
  padding: 1rem;
  margin-left: auto;
  margin-right: auto;
  
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
  /* background-color: white; */
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