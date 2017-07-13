<template>
            <div class="slider ui segment inverted container fluid">
                <span id="slider-arrow-left" @click="prev()"><i class="icon arrow left big"></i></span>
                <span id="slider-arrow-right" @click="next()"><i class="icon arrow right big"></i></span>
                <div class="ui grid centered">
                    <div class="slider-item" v-for="(img, index) in imgList">
                        <img :src="img" alt="" v-if="isBetween(index)">
                    </div>
                </div>
            </div>

</template>
<script>
  export default{
    props: {
      imgList: {}
    },
    methods: {
      prev: function () {
        let temp = this.imgList.shift()
        this.imgList.push(temp)
      },
      next: function () {
        let temp = this.imgList.pop()
        this.imgList.unshift(temp)
      },
      isBetween: function (index) {
        return index > 0 && index <= 3
      }
    }
  }
</script>

<style lang="scss">
    @mixin arrow {
        position: absolute;
        bottom: 50%;
        transform: translateY(50%);
        cursor: pointer;
    }
    .slider {
        position: relative;
        #slider-arrow-left{
            @include arrow;
            left: 0;
        }
        #slider-arrow-right{
            @include arrow;
            right: -3px;
        }
    }
</style>
