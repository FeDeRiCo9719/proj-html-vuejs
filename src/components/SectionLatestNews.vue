<template>
  <div class="latestNews">
    <div class="container">
      <!-- TITLE -->
      <div class="title">
        <h5 class="h5style">PHASELLUS EGET METUS</h5>
        <h2>All the latest news</h2>
        <hr class="HRstyle">
      </div>

      <!-- ROW IMAGES -->
      <div class="rowImages">
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

      <!-- HERO -->
      <div class="HeroNews hero1">
        <h5 class="h5style">PHASELLUS EGET METUS</h5>
        <h2>Cras malesuada et orci eget pharetra</h2>
        <p>Apsum dolor sit amet consectetur, adipisicing elit. E est voluptatum aspernatur, voluptatibus doloremque voluptates! Fuga eligendi laborum enim doloribus necessitatibus nam vel delectus, dolorem deleniti praesentium.</p>
        <div>
          <button  class="btnStyle blackBtn paddingBtn">
            READ MORE <i class="fas fa-chevron-right"></i>
          </button>
        </div>  
      </div>

      <!-- ROW IMAGES -->
      <div class="rowImages">
        <div v-for="(item, index) in imagesRow2" :key="index">
          <div class="boxImg">
            <img :src="require(`../assets/img/${item.img}.jpg`)" alt="imageNews">
          </div>
          <h4>{{item.title}}</h4>
          <div class="date">{{item.date}}</div>
          <p>{{item.text}}</p>
        </div>
      </div>

      <!-- HERO AND IMAGES -->
      <div class="hero_images">
        
        <!-- hero -->
        <div class="HeroNews hero2">
          <h5 class="h5style">PHASELLUS EGET METUS</h5>
          <h2>Cras malesuada et orci eget pharetra</h2>
          <p>Apsum dolor sit amet consectetur, adipisicing elit. E est voluptatum aspernatur, voluptatibus doloremque voluptates! Fuga eligendi laborum enim doloribus necessitatibus nam vel delectus, dolorem deleniti praesentium.</p>
          <div>
            <button  class="btnStyle blackBtn paddingBtn">
              READ MORE <i class="fas fa-chevron-right"></i>
            </button>
          </div>
        </div>

        <!-- images -->
        <div class="tutorialsBox">
          <h3>Tutorials & Guides</h3>
          <hr class="HRstyle">
          <Tutorial :TutorialsInfo="TutorialsInfo" />
        </div> 

      </div>
    </div>
  </div>
</template>

<script>
import Tutorial from './Tutorial.vue'

export default {
  name: 'SectionLatestNews',
  components: {
    Tutorial,
  },
  props: ['imagesRow1', 'imagesRow2'],
  data() {
    return {
      TutorialsInfo: [
        {
          img: 'post_feat_img_23-147x118',
          title: 'E est voluptatum  doloremque dolor sit aepe tenetu',
          date: 'October 11th, 2015 | Comments',
        },
        {
          img: 'post_feat_img_22-147x118',
          title: 'Lorem ipsum est tatibus doloremque aepe tenetu',
          date: 'October 11th, 2015 | Comments',
        },
        {
          img: 'post_feat_img_20-147x118',
          title: 'Voluptatum aspernatur dolor sit aepe tenetu',
          date: 'October 11th, 2015 | Comments',
        }
      ]
    }
  }
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
      margin: 0 auto;
    }
  }

  // three images
  .rowImages {
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
      font-size: 18px;
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

  // hero
  .HeroNews {
    background-color: rgb(146, 65, 65);
    color: white;
    padding: 0 100px;

    h2 {
      font-size: 30px;
      font-weight: 900;
    }
  }
  .hero1 {
    height: 600px;
    background-image: url('../assets/img/featured_article_1_bg.jpg');
    background-position: center;
    background-size: 100%;

    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    gap: 20px;
    padding-bottom: 100px;
  }
  .hero2 {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 20px;

    height: 500px;
    width: calc(100% - 100%/3);
    background-image: url('../assets/img/featured_article_2_bg.jpg');
    background-position: center;
    background-size: 100%;
  }

  // hero and images
  .hero_images {
    display: flex;
    gap: 50px;
    

    .tutorialsBox {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      width: calc(100%/3);

      h3 {
        font-size: 30px;
        font-weight: 900;
      }
      hr {
        margin: 30px 0;
      }
    }  
  }

}
</style>
