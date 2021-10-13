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
        <h5 class="h5style">AVADA FORUM IS THE PLACE TO BE</h5>
        <div class="BoxP">
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus sit odit maiores excepturi quos recusandae ipsam pariatur id eligendi sint qui, ad quibusdam iusto similique soluta ipsum deleniti voluptas temporibus.</p>
        </div>
      </div>
    </div>

    <!-- LATEST NEWS -->
    <SectionLatestNews :imagesRow1="imagesRow1" :imagesRow2="imagesRow2" />

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
import SectionLatestNews from './SectionLatestNews.vue'

export default {
  name: 'Main',
  components: {
    SectionLatestNews,
  },
  props: [],
  data() {
    return {
      imagesRow1: [
        {
          img: 'post_feat_img_25-320x202',
          title: 'Lorem ipsum dolor sit aepe tenetu',
          date: 'October 11th, 2015 | Comments',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing el torro odit officiis fugiat, quae quas, dolores dicta odio tempore hico aut blanditiis? Consectetur natus, ullam ducimus aliquid quisquam tenetur vel nisi.',
        },
        {
          img: 'post_feat_img_24-320x202',
          title: 'Lorem ipsum dolor sit aepe tenetu',
          date: 'October 11th, 2015 | Comments',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing el torro odit officiis fugiat, quae quas, dolores dicta odio tempore hico aut blanditiis? Consectetur natus, ullam ducimus aliquid quisquam tenetur vel nisi.',
        },
        {
          img: 'post_feat_img_23-320x202',
          title: 'Lorem ipsum dolor sit aepe tenetu',
          date: 'October 11th, 2015 | Comments',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing el torro odit officiis fugiat, quae quas, dolores dicta odio tempore hico aut blanditiis? Consectetur natus, ullam ducimus aliquid quisquam tenetur vel nisi.',
        }
      ],

      imagesRow2: [
        {
          img: 'post_feat_img_22-320x202',
          title: 'Lorem ipsum dolor sit aepe tenetu',
          date: 'October 11th, 2015 | Comments',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing el torro odit officiis fugiat, quae quas, dolores dicta odio tempore hico aut blanditiis? Consectetur natus, ullam ducimus aliquid quisquam tenetur vel nisi.',
        },
        {
          img: 'post_feat_img_21-320x202',
          title: 'Lorem ipsum dolor sit aepe tenetu',
          date: 'October 11th, 2015 | Comments',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing el torro odit officiis fugiat, quae quas, dolores dicta odio tempore hico aut blanditiis? Consectetur natus, ullam ducimus aliquid quisquam tenetur vel nisi.',
        },
        {
          img: 'post_feat_img_20-320x202',
          title: 'Lorem ipsum dolor sit aepe tenetu',
          date: 'October 11th, 2015 | Comments',
          text: 'Lorem ipsum dolor sit amet consectetur adipisicing el torro odit officiis fugiat, quae quas, dolores dicta odio tempore hico aut blanditiis? Consectetur natus, ullam ducimus aliquid quisquam tenetur vel nisi.',
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// HERO
.bgHero {
  padding-top: 100px;
  height: 800px;
  background-color: grey;
  color: white;

  background-image: url('../assets/img/home_slider_bg.jpg');
  background-position: center;
  background-size: 100%;
  
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
  text-align: center;
  padding: 100px 0;

  .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 20px;

    .BoxP {
      font-size: 20px;
      max-width: 50%;
      font-weight: 300;
    }
  }
}

</style>
