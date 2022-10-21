<script setup>
  import { ref } from 'vue';
  import ShowItem from './components/ShowItem.vue';
  import AddItem from './components/AddItem.vue';
  import Ballot from './components/stage/Ballot.vue';
</script>

<template>
  <div id="rootDIV main">
    <div id="operation-div">
      <AddItem id="add-item"></AddItem>
      <Ballot></Ballot>
    </div>
  </div>
</template>

<style lang="css"> 
.main{
  text-align: center;
  background-color: #fff;
  border-radius: 20px;
  width: 300px;
  height: 350px;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%,-50%);
}


#add-item {
  margin-bottom: 50px;
}

#watch-div {
  /* margin-right: 20em; */
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