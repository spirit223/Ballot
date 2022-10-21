<script setup>
  
</script>

<template>
  <div>
    <input class="itemInput" type="text" placeholder="请输入项目">
    <button class="radioBtn">D</button>
    <button class="radioBtn">C</button>
  </div>
</template>

<style lang="css">
  input {
    margin-left: 5px;
    margin-top: 5px;
    margin-right: 10px;
  }

  input:focus {
    border: none;
    border-bottom: rgb(255, 158, 191) solid 1px;
    outline: none;
    caret-color:red;
  }

  input::placeholder {
    color: rgb(73, 73, 73);
    font-size: 500;
  }
  
  .itemInput {
    height: 50px;
    border: none;
    width: 240px;
    border-radius: 25px;
    vertical-align: top;
    text-indent:20px;
  }

  button {
    margin: 5px;
  }

  .radioBtn {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background-color: rgba(35, 217, 110, 0.8);
    color: rgb(239, 234, 234);
    border: none;
    font-weight: 700;
    font-size: xx-large;
  }
</style>