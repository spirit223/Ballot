<script setup>
  import { ref } from 'vue';
  import ShowItem from './components/ShowItem.vue';
  import AddItem from './components/AddItem.vue';
  import Ballot from './components/stage/Ballot.vue';
</script>

<template>
  <div id="rootDIV">
    <div id="operation-div">
      <AddItem id="add-item"></AddItem>
      <Ballot></Ballot>
    </div>
    <div id="watch-div">
      <ShowItem></ShowItem>
    </div>
  </div>
</template>

<style lang="css">
#add-item {
  margin-bottom: 50px;
}

#watch-div {
  margin-left: 40em;
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