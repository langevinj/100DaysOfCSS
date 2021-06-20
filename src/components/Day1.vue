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
        margin-left: -2.3em;
        width: 4.6em;
        height: 0.54em;
        border-radius: 5px;
        box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
        position: absolute;
    }

    .top {
        background-color: white;
        margin-top: -0.54em;
        z-index: 100;
    }

    .middle {
        margin-top: 0.56em;
        background-color: white;
    }

    .bottom {
        background-color: white;
        margin-top: 1.66em;
    }

    a:focus > .middle {
        animation-name: middleAnimation;
        animation-duration: 0.5s;
        transition:width 1s ease-in-out;
    }

    a:focus > .top {
        animation-name: topAnimation;
        animation-duration: 0.5s;
        transition: 1s ease-in-out;
    }

    a:focus > .bottom {
        animation-duration: 0.5s;
        animation-name: bottomAnimation;
        transition: 1s ease-in-out;
    }

    @keyframes topAnimation {
        0% {
            margin-top: -0.54em;
            transform: rotate(0);
        }

        25% {
            margin-top: .56em;
            transform: rotate(0);
        }

        50% {
            margin-top: 0.56em;
            transform: rotate(0);
        }

        75% {
            margin-top: 0.56em;
        }

        100% {
            margin-top: 0.56em;
            transform: rotate(135deg)
        }
    }

    @keyframes bottomAnimation { 
        0% {
            margin-top: 1.66em;
            transform: rotate(0);
        }

        25% {
            margin-top: 1.1em;
            transform: rotate(0);
        }

        50% {
            margin-top: 0.56em;
            transform: rotate(0);
        }

        75% {
            margin-top: 0.56em;
        }

        100% {
            margin-top: 0.56em;
            transform: rotate(45deg)
        }
    }

    @keyframes middleAnimation {
       0% {
          margin-left: -2.3em;
          margin-right: -2.3em;
          width: 4.6em;
       } 

       25% {
           margin-left: -1.15em;
           margin-right: -1.15em;
           width: 2.3em;
       }

       50% {
          margin-left: -0em;
          margin-right: -0em;
          width: 0em;
          display: none;
       }

       75% {
           display: none;
       }

       100% {
           display: none;
       }
    }

    a:focus > .top {
        transform: rotate(135deg);
        margin-top: 0.56em;
    }

    a:focus .bottom { 
        margin-top: 0.56em;
        transform: rotate(45deg)
    }

    a:focus .middle {
        display: none;
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