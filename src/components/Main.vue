<template>
  <main>
    <!-- HERO -->
    <div class="bgHero">
      <div class="container">
        <h1>Tech Forum!</h1>
        <p>Discuss all the latest technology news and trends</p>
        <div>
          <button  class="btnStyle colorBtn paddingBtn">
            GET AVADA NOW! <i class="fas fa-chevron-right"></i>
          </button>
        </div>       
      </div>
    </div>

    <!-- DESCRIPTION -->
    <div class="description">
      <div class="container">
        <h5>AVADA FORUM IS THE PLACE TO BE</h5>
        <div class="BoxP">
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus sit odit maiores excepturi quos recusandae ipsam pariatur id eligendi sint qui, ad quibusdam iusto similique soluta ipsum deleniti voluptas temporibus.</p>
        </div>
      </div>
    </div>

    <!-- LATEST NEWS -->
    <div class="latestNews">
      <div class="container">
        
      </div>
    </div>

    <!-- blackBar -->
    <!-- FORUM SECTION -->
    <div class="">
      <div class="container">
        
      </div>
    </div>
    <!-- blackBar -->

    <!-- JOIN COMMUNITY -->
    <div class="">
      <div class="container">
        
      </div>
    </div>

    <!-- NEWSLETTER -->
    <div class="">
      <div class="container">
        
      </div>
    </div>

  </main>
</template>

<script>
export default {
  name: 'Main',
  props: []
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// HERO
.bgHero {
  padding-top: 100px;
  height: 800px;
  background-color: grey;
  // background-image: url();
  color: white;
  
  .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 40px;

    h1 {
      font-size: 120px;
      line-height: 92px;
      // background-color: rgb(255, 166, 0);
    }
    p {
      font-size: 25px;
      font-weight: 300;
    }
  }
}

// DESCRIPTION
.description {
  background-color: rgb(219, 218, 214);
  height: 300px;
  text-align: center;

  .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 20px;

    h5 {
      font-weight: 900;
    }

    .BoxP {
      font-size: 20px;
      max-width: 50%;
      font-weight: 300;
    }
  }
}

//LATEST NEWS 
.latestNews {
  background-color: white;
  height: 2000px;
}


</style>
