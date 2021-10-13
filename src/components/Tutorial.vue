<template>
  <div class="box">
    <div class="singleBox" v-for="( item, index ) in TutorialsInfo" :key="index">
      <img :src="require(`../assets/img/${item.img}.jpg`)" alt="tutorial Img"> 
      <!-- <img :src="`../assets/img/${item.img}.jpg`" alt="tutorial Img"> -->
      <!-- <img :src="('../assets/img/' + item.img + '.jpg')" alt="tutorial Img"> -->
      <div>
        <h4>{{item.title}}</h4>
        <div class="date">{{item.date}}</div>
      </div>  
    </div>
  </div>
</template>

<script>
export default {
  name: 'Tutorial',
  props: ['TutorialsInfo']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.box {
  display: flex;
  flex-direction: column;
  gap: 20px;

  .singleBox {
    display: flex;
    gap: 20px;
  
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
  }
}
</style>
