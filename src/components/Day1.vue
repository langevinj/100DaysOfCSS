<template>
    <div class="frame">
        <div class="center">
        <a href="#">
            <div class="bar top"></div>
            <div class="bar middle"></div>
            <div class="bar bottom"></div>
        </a>
        </div>
    </div>
</template>

<style scoped src="../assets/styles/day1.css"></style>

<script>
</script>

<style scoped>
    .top, .middle, .bottom {
        left: 50%;
        width: 75px;
        margin-bottom: 12px;
        height: 7px;
        background-color: white;
        border-radius: 5px;
        box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
        top: 50%;
    }

    .middle {
        margin: 12px auto;
    }

    a:focus > .middle {
        animation-name: example;
        animation-duration: 0.25s;
        transition:width 1s ease-in-out;
    }

    @keyframes example {
       0% {
          transform: scaleX(1);
       } 

       25% {
           transform: scaleX(.5);
       }

       50% {
           transform: scaleX(.50);
       }

       75% {
           width: 0;
       }

       100% {
          width: 0;
       }
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