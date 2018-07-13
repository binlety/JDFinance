<template lang="html">
        <Panel title="新品推荐" :class="$style.panel">
                <section :class="$style.content">
                    <div :class="$style.arrow">更多尖货 ></div>
                    <Slider :options="options" :items="items" cname="product-slider"></Slider>
                </section>
        </Panel>
</template>

<script>
import Panel from "../core/panel.vue";
import Slider from "../core/slider.vue";
export default {
    components:{
        Panel,
        Slider
    },
    data(){
        return {
            items:[
                {
                    id:1,
                    href:"home",
                    src:"//img12.360buyimg.com/jrpmobile/jfs/t20368/53/1699227456/59616/e6a80ca4/5b30a580N130c8dfc.jpg"
                },
                 {
                    id:2,
                    href:"home",
                    src:"//img12.360buyimg.com/jrpmobile/jfs/t23338/182/473320295/44592/4835b8d8/5b30a593N32e80321.jpg"
                },
                 {
                    id:3,
                    href:"home",
                    src:"//img12.360buyimg.com/jrpmobile/jfs/t23323/199/462493049/28263/3d0f7cbf/5b30a5a5N3dec8fdc.jpg"
                },
                 {
                    id:4,
                    href:"home",
                    src:"//img12.360buyimg.com/jrpmobile/jfs/t20368/53/1699227456/59616/e6a80ca4/5b30a580N130c8dfc.jpg"
                }
            ],
            options:{
                slidesPerView:2.3,
                spaceBetween:30,
                loop:true,
                freeMode:true
            }
        }
    }
}
</script>

<style lang="scss" module>
    @import "../../css/element.scss";
    .panel{
        @include panel;
        .content{
            padding-bottom: 40px;
            position: relative;
            &>div{
                position: absolute;
                font-size: 28px;
                color: #999;
                right: 20px;
                top: -70px;
            }
        }
    }  
  
</style>

<style lang="scss">
      .product-slider{
        .swiper-container{
            box-sizing: border-box;
            padding:0 24px;
            .swiper-slide{
                a{
                    display: inline-block;
                    width:100%;
                    img{
                        width:100%;
                        display: block;
                        height: 314px;
                        border:1px solid #fafafa;
                    }
                }
            }
        }
    }
</style>
