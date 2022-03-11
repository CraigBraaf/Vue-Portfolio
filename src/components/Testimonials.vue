<template>
<section id="testimonials">
<div class="testimonials-heading">
        <h1>TESTIMONIALS</h1>
      </div>
      <div class="testimonials-container">
        <div class="testimonial" v-for="testimonial of testimonials" :key="testimonial">
          <div class="testimonial-image">
            <img :src="testimonial.img" :alt="testimonial.name" />
          </div>
          <div class="testimonial-content">
            <h2>{{ testimonial.name }}</h2>
            <p>{{ testimonial.description }}</p>
            <cite>{{ testimonial.position }}</cite>
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

#testimonials {
    background-color:  rgb(95, 93, 93);
    /* height: 100vh; */

}

.testimonials-heading h1 {
    padding-top: 5rem;
    margin-bottom: 5rem;
    color: white;
  }

  .testimonials-container {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-around;
    flex-direction: row;
    flex-wrap: wrap;
    padding-bottom: 5rem;
    margin-left: 50px;
    margin-right: 50px;
    
  }

  .testimonial {
    width: 25%;
    height:50vh;
    display: flex;
    flex-direction: column;
    color: #000;
    border-radius: 5px;
    box-shadow: rgba(17, 17, 26, 0.1) 0px 0px 16px;
    margin: 10px;
    background: rgba(255, 255, 255);
  }

  .testimonial-image {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 20px;
  }

  .testimonial-image img {
    width: 65%;
    border-bottom-right-radius: 50%;
    border-top-left-radius: 50%;
    border-top-right-radius: 5%;
    border-bottom-left-radius: 5%;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  }

  .testimonial-content {
    padding: 50px;
    margin-top: auto;
    margin-bottom: auto;
    display: flex;
    flex-direction: column;
  }

  .testimonial-content p {
    line-height: 25px;
  }

  @media only screen and (max-width: 1100px) {
    .testimonials-container {
      width: 80%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-direction: column;
      flex-wrap: wrap;
      gap: 2rem;
      margin-left: 20px;
      margin-right: 20px;
    }

    .testimonial {
      width: 100%;
      display: flex;
      flex-direction: row;
      color: #000;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 25);
    }

    .testimonial-image {
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 25px;
    }

    .testimonial-image img {
      width: 100%;
    border-bottom-right-radius: 50%;
    border-top-left-radius: 50%;
    border-top-right-radius: 5%;
    border-bottom-left-radius: 5%;
    }

    .testimonial-content {
      width: 100%;
      padding: 20px;
      display: flex;
      justify-content: center;
      align-items: flex-start;
      flex-direction: column;
      text-align: initial;
    }
  }

  @media only screen and (max-width: 770px) {

    .testimonials-container {
      width: 85%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-direction: column;
      flex-wrap: wrap;
      gap: 2rem;
      margin-left: 20px;
    }

    .testimonial {
      width: 92%;
      height: auto;
      display: flex;
      flex-direction: row;
      color: #000;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 25);
    }

    .testimonial-image {
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 25px;
    }

    .testimonial-image img {
      width: 90%;
          border-bottom-right-radius: 50%;
    border-top-left-radius: 50%;
    border-top-right-radius: 5%;
    border-bottom-left-radius: 5%;
    }

    .testimonial-content {
      width: 100%;
      padding: 20px;
      display: flex;
      justify-content: center;
      align-items: flex-start;
      flex-direction: column;
    }
  }

  @media only screen and (max-width: 576px) {
    .testimonials-container {
      width: 75%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-direction: column;
      flex-wrap: wrap;
      gap: 0.5rem;
      margin-left: 10px;
    }

    .testimonial {
      width: 100%;
      height: auto;
      display: flex;
      flex-direction: column;
      color: #000;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 25);
    }

    .testimonial-image {
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 25px;
    }

    .testimonial-image img {
      width: 80%;
      border-radius: 10px;
    }

    .testimonial-content {
      width: 100%;
      padding: 25px;
      display: flex;
      justify-content: center;
      align-items: flex-start;
      flex-direction: column;
    }

    .testimonials-heading h1 {
      font-weight: 900;
      font-size: 35px;
      color: #000;
      margin-top: 5rem;
      margin-bottom: 5rem;
      text-align: center;
    }

    .testimonials-heading {
      width: 100%;
      padding: 25px;
    }
  }



</style>