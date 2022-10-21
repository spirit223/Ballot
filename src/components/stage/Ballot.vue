<script setup>
  import { ref } from 'vue';
  const showItem = ref('点击按钮抽签')
  const items = ref([
    '尽力撕掉对方丝袜或衣物',
    '把酒倒在自己身上对方舔干',
    '亲吻对方胸部',
    '被对方摸撩2分钟不得反抗',
    '舔对方丝足或手指',
    '挑逗对方敏感部位',
    '侧抱相互喂酒喂吃',
    '女方被男方公主抱在屋内走一圈',
    '想办法弄对方下面有反应',
    '嘴里含着水亲吻对方身体1分钟',
    '依次亲吻对方额头鼻子嘴唇脖子',
    '深情亲吻对方30s',
    '躺下享受被对方舔遍全身5分钟',
    '亲吻对方大腿内测',
    '用跳蛋按摩对方身体敏感部位',
    '舔对方耳朵',
    '按对方要求穿上指定的情趣内衣',
    '穿上丝袜用脚按摩男方丁丁1分钟',
    '对方口你下面',
    '对从对方的任何要求'
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
    <button @click="randomItem">random</button>
    <div id="exhibit">
      {{ showItem }}
    </div>
  </div> 
</template>

<style lang="css">
html,body {
  background-color: rgb(51, 51, 51);
}

#ballot-root{
  background-color: rgb(51, 51, 51); 
}
#ballot-root > button {
  width: 200px;
  font-size: 40px;
  margin-left: 150px;
  border-radius: 20px;
  background-color: rgb(141, 193, 72);
  border: none;
}
#exhibit {
  font-size: 26px;
  color: lightcoral;
  display: flex;
  justify-content: center;
  align-items:center;
  height: 200px;
  width: 500px;
  background-color: darkseagreen;
}
</style>