<template>
  <section id="Projects">
    <br><br><br>
      This is my Projects
  <div class="grid">
        <div class="grid-item">
          <div class="procard">
               <img class="procard-img" src="1stPortfolio.png" alt="Mockport" />
               <div class="procard-content">
                <h1 class="procard-header"> Secondary Portfolio <br></h1>
                <p class="procard-text">
                  Project consist of my First ever Portfolio Website
                </p>
                <a href="https://github.com/HaniJar/My-Portfolio" target="_blank"><button id="da-btn" class="btn btn-secondary" type="button">Github</button></a>
                <a href="https://modest-jepsen-572175.netlify.app/" target="_blank"><button id="da-womb" class="btn btn-secondary" type="button">Netlify</button></a>
               </div> 
          </div>
        </div>
      </div>
      </section>
</template>

<script>
// export default {
//     data() {
//         return {
//             id: 1,
//             name: ,
//             url: 
//         }
//     }
// }
</script>

<style>

 #Projects {
    background-color: red;
    background-image: linear-gradient(to top right, yellow, red);
    background-size: cover;
    background-repeat: no-repeat;
    height: 100vh;
  }

.grid {
    margin-top: 80px;
    margin-left: 160px;
    margin-right: 50px;
    display: inline-block;
    width: 20%;
    grid-gap: 6rem;
    grid-template-columns: repeat(auto-fit, minmax(30rem, 1fr));
    align-items: start;
}

.grid-item {
    background-color: #fff;
    border-radius: 0.4rem;
    overflow: hidden;
    box-shadow: 0 3rem 6rem rgba(0, 0, 0, 0.1);
    cursor:pointer;
    transition: 0.2s;
}

.grid-item:hover {
    transform: translateY(-0.5%);
    box-shadow: 0 4rem 8rem rgba(0, 0, 0,0.5);
}

.procard-img {
    display: block;
    width: 100%;
    height: 15rem;
    object-fit:cover;
}


 
</style>