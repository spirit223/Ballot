<script setup>
  import { ref } from 'vue';
  const showItem = ref('点击 random 按钮抽签')
  const items = ref([
  ])

  function randomItem() {
    let index = getRandomInt(0, items.value.length)
    showItem.value = items.value[index]
  }
  
  /**
   * 获取两个数之间的随机整数
   * @param {Number} min 随机整数的下界, 包含
   * @param {Number} max 随机整数的上界, 不包含
   */
  function getRandomInt(min, max) {
    min = Math.ceil(min);
    max = Math.floor(max);
    return Math.floor(Math.random() * (max - min)) + min; //不含最大值，含最小值
  }
</script>

<template>
  <div id="ballot-root">
    <button @click="randomItem" id="randonBtn">RANDOM</button>
    <div id="exhibit">
      {{ showItem }}
    </div>
  </div> 
</template>

<style lang="css">
/* html,body {
  background-color: rgb(51, 51, 51);
} */

#ballot-root{
  background-color: rgb(44, 100, 63); 
  border-radius: 10px;
}
#ballot-root > button {
  color: rgb(255, 255, 255);
  width: 200px;
  font-size: 40px;
  margin-left: 150px;
  margin: 10px 0px 10px 150px;
  border-radius: 20px;
  background-color: rgb(133, 180, 102);
  border: none;
}
#exhibit {
  font-size: 26px;
  color: rgb(255, 255, 255);
  display: flex;
  justify-content: center;
  align-items:center;
  height: 200px;
  width: 500px;
  background-color: rgb(133, 180, 102);
  border-bottom-left-radius: 10px;
  border-bottom-right-radius: 10px;
}
</style>