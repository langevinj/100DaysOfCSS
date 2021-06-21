<template>
    <div class="circle">
        <div class="segment-top"></div>
        <div class="triangle"></div>
        <div class="segment-bottom"></div>
    </div>
</template>

<script>

</script>

<style scoped>
    .circle {
        height: 180px;
        width: 180px;
        border-radius: 50%;
        background-color: white;
        position: absolute;
        margin-top: -100px;
        margin-left: -90px;
        overflow: hidden;
    }

    .triangle {
      width: 0;
      height: 0;
      border: 65px solid transparent;
      border-bottom-color: white;
      top: 0px;
      left: 25px;
      position: absolute;
    }

   .segment-top {
        float: left;
        width: 100%;
        height: 300px;
        background: #7BDBF8;
        margin-bottom: 0;
        position: absolute;
    }

    .segment-bottom {
        float: left;
        width: 100%;
        height: 100px;
        margin-top: 120px;
        background: #DFCF6F;
        z-index: 20;
        position: absolute;
    }
</style>