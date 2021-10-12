<template>
  <header>
    <div class="container">

      <!-- logo -->
      <div class="logoBox">
        <img src="../assets/img/logo.png" alt="logo">
      </div>

      <div class="Nav">
        <!-- nav -->
        <nav>
          <ul>
            <li v-for="(link, index) in navLinks" :key="index">
              <a :href="link.url">{{link.text}}</a>
            </li>
          </ul>
        </nav>
      
        <!-- join us button -->
        <button class="btnStyle blackBtn">
          JOIN US
        </button>

        <!-- searchbar -->
        <div>
          <i class="fas fa-search"></i>
        </div>
      </div>

    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: ['navLinks']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  height: 100px;
  width: 100%;
  position: fixed;
  z-index: 10;
  color: white;

  .btnStyle {
    padding: 10px 15px;
    margin-right: 50px;
  }

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .logoBox {
      height: 60px;
      cursor: pointer;
      img {
        height: 100%;
      }
    }

    .Nav {
      height: 100%;
      display: flex;
      justify-content: space-between;
      align-items: center;

      li {
        display: inline-block;
        margin-right: 50px;

        a {
          color: white;
          
          &:hover {
            transition: 0.2s;
            color: rgb(224, 224, 224);
          }
        }
      }
    }
    .fa-search {
      cursor: pointer;

      &:hover {
        transition: 0.2s;
        color: rgb(224, 224, 224);
      }
    }
  }
}
</style>
