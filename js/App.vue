<template>
    <div id="app">
        <div id="header">
            <div id="header-bg" class="pos-rel">
                <div class="pos-abs-middle-center anim-top">
                    LES POUPONS DE TERANGA
                </div>
            </div>
        </div>
        <div id="donnation">
            <a class="ui button blue " href="">Aidez-nous</a>
        </div>
        <div class="ui container">
            <div class="ui segment" id="homepage-first-desc">
                <div class="ui grid">
                    <div class="four wide column">
                        <div class="ui fluid image">
                            <img src="http://via.placeholder.com/300x200">
                        </div>
                    </div>
                    <div class="twelve wide column">
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci aliquid amet autem,
                            corporis debitis dignissimos iste iusto modi necessitatibus nemo neque, numquam odio officia
                            optio qui reprehenderit ullam veniam veritatis!
                        </p>
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci aliquid amet autem,
                            corporis debitis dignissimos iste iusto modi necessitatibus nemo neque, numquam odio officia
                            optio qui reprehenderit ullam veniam veritatis!
                        </p>
                    </div>

                </div>
            </div>
            <div class="ui equal height grid">
                <div class="six wide column">
                    <div class="ui fluid image">
                        <img src="http://via.placeholder.com/300x200">
                    </div>
                </div>
                <div class="ten wide column stretched">
                    <div class="ui segment">
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. A consectetur cumque ea earum, est
                            facere nemo quae quaerat quia tempora tempore vel? Commodi consequatur corporis illo magnam
                            pariatur praesentium voluptatem.
                        </p>
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. A consectetur cumque ea earum, est
                            facere nemo quae quaerat quia tempora tempore vel? Commodi consequatur corporis illo magnam
                            pariatur praesentium voluptatem.
                        </p>
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. A consectetur cumque ea earum, est
                            facere nemo quae quaerat quia tempora tempore vel? Commodi consequatur corporis illo magnam
                            pariatur praesentium voluptatem.
                        </p>
                    </div>
                </div>
            </div>
        </div>
        <slider :imgList="imgList"></slider>
    </div>

</template>

<script>
  import Slider from './components/slider/slider.vue'
  export default {
    name: 'app',
    data () {
      return {
        imgList: [
          '/img/300.jpeg',
          '/img/300-2.jpeg',
          '/img/300-3.jpeg',
          '/img/300-4.jpeg',
          '/img/300-5.jpeg'
        ]
      }
    },
    components: {
      slider: Slider
    }
  }
</script>
