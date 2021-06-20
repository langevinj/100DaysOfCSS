<template>
    <div class="frame">
        <div class="center">
            <div class="bar"></div>
            <div class="bar"></div>
            <div class="bar"></div>
        </div>
    </div>
</template>

<style scoped src="../assets/styles/day1.css"></style>

<script>
</script>

<style scoped>
    .bar {
        background-color: white;
        width: 75px;
        height: 7px;
        margin-bottom: 12px;
        border-radius: 5px;
        box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
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
    background: #6EBA8A;
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