<template>
    <div class="circle">
        <div class="segment-top"></div>
        <div class="sun"></div>
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

    .sun {
        background: yellow;
        position: absolute;
        border-radius: 50%;
        width: 35px;
        height: 35px;
        z-index: 30;
        top: 15px;
        left: 120px;
        animation: 3s ease-in-out 0s infinite sunAnimation;
    }

    @keyframes sunAnimation {
        0% {
            top: 65px;
            left: -30px;
        }

        25% {
            top: 15px;
            left: 20px;
        }

        50% {
            top: 15px;
            left: 20px;
        }

        75% {
            top: 15px;
            left: 120px;
        }

        100% {
            top: 65px;
            left: 175px;
        }


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