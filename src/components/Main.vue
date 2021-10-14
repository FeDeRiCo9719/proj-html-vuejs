<template>
  <main>
    <!-- HERO section -->
    <section class="bgHero">
      <div class="container">
        <h1>Tech Forum!</h1>
        <p>Discuss all the latest technology news and trends</p>
        <div>
          <button  class="btnStyle colorBtn paddingBtn">
            GET AVADA NOW! <i class="fas fa-chevron-right"></i>
          </button>
        </div>       
      </div>
    </section>

    <!-- DESCRIPTION section -->
    <section class="bgColor centerBox">
      <div class="textBox">
        <h5 class="h5style">AVADA FORUM IS THE PLACE TO BE</h5>        
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus sit odit maiores excepturi quos recusandae ipsam pariatur id eligendi sint qui, ad quibusdam iusto similique soluta ipsum deleniti voluptas temporibus.</p>        
      </div>
    </section>

    <!-- LATEST NEWS section -->
    <SectionLatestNews :imagesRow1="imagesRow1" :imagesRow2="imagesRow2" />

    <!-- blackBar -->
    <div class="blackBar centerBox">
      <h4>READ OUR BLOG</h4>
      <i class="fas fa-long-arrow-alt-right"></i>
    </div>

    <!-- FORUM section -->
    <section class="forumSection bgColor">
      <div class="container">
        <!-- title -->
        <div class="title">
          <h5 class="h5style">PHASELLUS EGET METUS</h5>
          <h2>Forum Sections</h2>
          <hr class="HRstyle">
        </div>
        <!-- items -->
        <div class="boxItems">
          <div class="item centerColumnBox">            
            <div class="bgCircle centerBox">
              <i class="fas fa-file-alt"></i>
            </div>
            <h5>News & Community</h5>           
          </div>

          <div class="item centerColumnBox">            
            <div class="bgCircle centerBox">
              <i class="fas fa-file-alt"></i>
            </div>
            <h5>News & Community</h5>           
          </div>
          <div class="item centerColumnBox">            
            <div class="bgCircle centerBox">
              <i class="fas fa-file-alt"></i>
            </div>
            <h5>News & Community</h5>           
          </div>
          
          <div class="item centerColumnBox">            
            <div class="bgCircle centerBox">
              <i class="fas fa-file-alt"></i>
            </div>
            <h5>News & Community</h5>           
          </div>
          <div class="item centerColumnBox">            
            <div class="bgCircle centerBox">
              <i class="fas fa-file-alt"></i>
            </div>
            <h5>News & Community</h5>           
          </div>
          
          <div class="item centerColumnBox">            
            <div class="bgCircle centerBox">
              <i class="fas fa-file-alt"></i>
            </div>
            <h5>News & Community</h5>           
          </div>             
        </div>
      </div>
    </section>

    <!-- blackBar -->
    <div class="blackBar centerBox">
      <h4>GO TO OUR FORUM</h4>
      <i class="fas fa-long-arrow-alt-right"></i>
    </div>

    <!-- JOIN COMMUNITY section -->
    <section class="bgJoinCommunity centerBox">      
      <div class="boxJoinCommunity">        
        <h2>Hey! Join to our Community</h2>       
        <p>Ratione dolores ipsum cumquent quos consectetur eum exercitationem natus. Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        <div>
          <button  class="btnStyle colorBtn paddingBtn">
            SIGN UP! <i class="fas fa-chevron-right"></i>
          </button>
        </div>
      </div> 
    </section>

    <!-- NEWSLETTER section -->
    <section class="bgColor centerBox">     
      <div class="boxNewsLetter">
        <h4>Subscribe to our Newsletter</h4>
        <div class="emailBox">
          <input type="text" placeholder="Insert your email*">
          <button  class="btnStyle blackBtn">SEND</button>
        </div>
      </div>     
    </section>

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
// hero section
.bgHero {
  padding-top: 220px;
  height: 900px;
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

// description section
.textBox {
  text-align: center;
  width: 40%;

  p {
    font-size: 20px;
    font-weight: 300;
    margin-top: 20px;
  }
}

// blackBar section
.blackBar {
  background-color: black;
  color: white;
  height: 100PX;
  gap: 10px;
}

// forumSection section
.forumSection {

  .container {
    display: flex;
    flex-direction: column;
    gap: 80px;
  }

  .title {
    text-align: center;
    background-color: rgba(69, 184, 24, 0.363);

    h2 {
      font-size: 40px;
      font-weight: 900;
      margin: 25px 0;
    }
    hr {
      margin: 0 auto;
    }
  }
  .boxItems {
    background-color: rgba(181, 184, 24, 0.363);
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 40px;

    .item {
      background-color: rgba(255, 255, 255, 0.363);
      border-top: 3px solid rgb(0, 173, 196);
      width: calc((100% - 120px) / 4);
      // width: 300px;
      height: 280px;

      .bgCircle {
        width: 80px;
        height: 80px;
        border-radius: 50%;
        background-color: chocolate;
        color:white;
        font-size: 24px;
      }
      h5 {
        font-size: 18px;
        text-align: center;
        font-weight: 900;
      }
    }
  }
}

// Join community section
.bgJoinCommunity {
  color: white;
  background-image: url('../assets/img/join_now_cta_bg.jpg');
  background-position: center;
  background-size: 100%;
  
  .boxJoinCommunity {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 30px;
    text-align: center;
    width: 500px;
  }
   
  h2 {
    font-size: 50px;
    font-weight: 900;
  }
  
}

// Newsletter section
.boxNewsLetter {
  text-align: center;
  width: 40%;
  // background-color: rgba(79, 79, 136, 0.514);

  h4 {
    font-size: 24px;
  }

  .emailBox {
    margin-top: 30px;
    width: 100%;
    height: 40px;
    // background-color: rgb(117, 211, 255);
    display: flex;
    gap: 20px;

    input {
      width: 70%;
      padding: 5px;
      border: 1px solid white;
      outline: none;
    }
    button {
      width: 30%;
    }
  }
 
}

</style>
