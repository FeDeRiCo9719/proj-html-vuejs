<template>
  <div class="latestNews">
    <div class="container">
      <!-- title -->
      <div class="title">
        <h5 class="h5style">PHASELLUS EGET METUS</h5>
        <h2>All the latest news</h2>
        <hr>
      </div>

      <!-- three images -->
      <div class="boxImages">
        <div v-for="(item, index) in imagesRow1" :key="index">
          <div class="boxImg">
            <img :src="require(`../assets/img/${item.img}.jpg`)" alt="imageNews">
            <!-- <img :src="`../assets/img/${item.img}.jpg`" alt="imageNews"> -->
          </div>
          <h4>{{item.title}}</h4>
          <div class="date">{{item.date}}</div>
          <p>{{item.text}}</p>
        </div>
      </div>

      <!-- little hero -->
      <div class="littleHero">
        <h5 class="h5style">PHASELLUS EGET METUS</h5>
        <h2>Cras malesuada et orci eget pharetra</h2>
        <p>Apsum dolor sit amet consectetur, adipisicing elit. E est voluptatum aspernatur, voluptatibus doloremque voluptates! Fuga eligendi laborum enim doloribus necessitatibus nam vel delectus, dolorem deleniti praesentium.</p>
        <div>
          <button  class="btnStyle blackBtn paddingBtn">
            READ MORE <i class="fas fa-chevron-right"></i>
          </button>
        </div>  
      </div>

      <!-- three images -->
      <div class="boxImages">
        <div v-for="(item, index) in imagesRow2" :key="index">
          <div class="boxImg">
            <img :src="require(`../assets/img/${item.img}.jpg`)" alt="imageNews">
            <!-- <img :src="`../assets/img/${item.img}.jpg`" alt="imageNews"> -->
          </div>
          <h4>{{item.title}}</h4>
          <div class="date">{{item.date}}</div>
          <p>{{item.text}}</p>
        </div>
      </div>

      <!-- hero and small images -->
      <div class=""></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SectionLatestNews',
  props: ['imagesRow1', 'imagesRow2']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.latestNews {
  background-color: white;
  padding: 120px 0;

  .container {
    display: flex;
    flex-direction: column;
    gap: 80px;
  }

  // title
  .title {
    text-align: center;
    h2 {
      font-size: 40px;
      font-weight: 900;
      margin: 25px 0;
    }
    hr {
      border-color: rgb(255, 123, 0);
      width: 80px;
      height: 1px;
      margin: 0 auto;
    }
  }

  // three images
  .boxImages {
    display: flex;
    justify-content: space-between;
    gap: 40px;

    .boxImg {
      width: 100%;
      margin-bottom: 20px;
      img {
        width: 100%;
      }
    }
    h4 {
      font-size: 20px;
      font-weight: 900;
      margin-bottom: 5px;
    }
    .date {
      font-size: 12px;
      margin-bottom: 10px;
      color: rgb(83, 83, 83);
    }
    p {
      color: rgb(83, 83, 83);
    }
  }

  // little hero
  .littleHero {
    height: 600px;
    background-color: grey;
    color: white;
    padding: 0 100px;

    background-image: url('../assets/img/featured_article_1_bg.jpg');
    background-position: center;
    background-size: 100%;

    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 20px;

    h2 {
      font-size: 30px;
      font-weight: 900;
    }
  }
  // three images

  // hero and small images

}
</style>
