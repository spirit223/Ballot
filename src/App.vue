<script setup>
  import { ref } from 'vue';
  import ShowItem from './components/ShowItem.vue';
  import AddItem from './components/AddItem.vue';
  import Ballot from './components/stage/Ballot.vue';
</script>

<template>
  <div id="rootDIV" class="main">
    <div id="operation-div">
      <AddItem id="add-item"></AddItem>
      <Ballot></Ballot>
    </div>
  </div>
</template>

<style lang="css">
.main{
  width: 300px;
  height: 350px;
  margin: 0 auto;
}


#add-item {
  margin: 20px;
}

#watch-div {
  display: inline-block;
}

#operation-div {
  display: inline-block;
}

#rootDIV {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>