<template>
  <div class="boxItems">
    <div class="item centerColumnBox" v-for="(item,index) in itemsForum" :key="index">            <!-- v-for="(item,index) in itemsForum" :key="index" -->
      <div class="bgCircle centerBox">
        <i :class="item.icon"></i>
      </div>
      <h5>{{ item.name }}</h5>           
    </div>
  </div>  
</template>

<script>
export default {
  name: 'ItemForum',
  props: ['itemsForum']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.boxItems {
  // background-color: rgba(181, 184, 24, 0.363);
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 40px;

  .item {
    background-color: white;
    border-top: 5px solid rgb(0, 155, 175);
    width: calc((100% - 120px) / 4);
    // width: 300px;
    height: 280px;

    .bgCircle {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      background-color: chocolate;
      color:white;
      font-size: 50px;
    }

    h5 {
      font-size: 20px;
      text-align: center;
      font-weight: 900;
    }
  }
}  
</style>
