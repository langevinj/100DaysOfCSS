<template>
<div class="frame">
  <div class="center">
    <Day2 />
  </div>
</div>
</template>

<script setup>
import Day1 from './components/Day1.vue';
import Day2 from './components/Day2.vue';

// This starter template is using Vue 3 experimental <script setup> SFCs
// Check out https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

 .frame {
    position: absolute;
    top: 50%;
    left: 50%;
    width: 400px;
    height: 400px;
    margin-top: -200px;
    margin-left: -200px;
    border-radius: 2px;
      box-shadow: 4px 8px 16px 0 rgba(0,0,0,0.1);
      overflow: hidden;
      /* background: #6EBA8A; */
      background: #272C34;
    color: #333;
      font-family: 'Open Sans', Helvetica, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
  }
  
.center {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
}
</style>
