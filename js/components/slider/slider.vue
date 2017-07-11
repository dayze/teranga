<template>
    <div class="ui container">
        <div class="slider">
            <span id="slider-arrow-left"><i class="icon arrow left big"></i></span>
            <span id="slider-arrow-right"><i class="icon arrow right big"></i></span>
            <div class="slider-item" v-for="img in imgList">
                {{ img }}
            </div>
        </div>
    </div>
</template>
<script>
  export default{
    props: {
      imgList: {}
    }
  }
</script>

<style lang="scss">
    .slider {
        display: flex;
        position: relative;
        #slider-arrow-left{
            position: absolute;
            bottom: 50%;
            left: 0;
            transform: translateY(50%);
        }
        #slider-arrow-right{
            position: absolute;
            bottom: 50%;
            right: -3px;
            transform: translateY(50%);
        }
        .slider-item {
            height: 200px;
            width: 250px;
            background-color: red;
        }
    }
</style>
