<script setup>
  
</script>

<template>
  <div>
    <div id="input-bar">
      <input class="itemInput" type="text" placeholder="请输入项目">
      <button class="radioBtn">D</button>
      <button class="radioBtn">C</button>
    </div>
  </div>
</template>

<style lang="css">
  #input-bar {
    width: 400px;
  }

  input {
    margin-left: 5px;
    margin-top: 5px;
    margin-right: 10px;
    background-color: rgb(250, 226, 93);
  }

  input:focus {
    border: none;
    border-bottom: rgb(255, 158, 191) solid 2px;
    outline: none;
    caret-color:red;
  }

  input::placeholder {
    color: rgb(73, 73, 73);
    font-size: 500;
  }
  
  .itemInput {
    /* margin-left: 100px; */
    margin-left: 100px;
    display: inline-block;
    height: 50px;
    border: none;
    width: 240px;
    border-radius: 25px;
    vertical-align: top;
    text-indent:20px;
  }

  button {
    display: inline-block;
    margin: 5px;
  }

  .radioBtn {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    border-bottom-right-radius: -50%;
    background-color: rgb(133, 180, 102);
    color: rgb(239, 234, 234);
    border: none;
    font-weight: 700;
    font-size: xx-large;
  }
</style>