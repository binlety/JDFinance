<template lang="html">
        <Panel title="轮播图" :class="$style.panel">
               <section :class="$style.content">
                   <Slider :items="items" :cname="$style.slider"/>
               </section>
        </Panel>
</template>

<script>
import Panel from "../core/panel.vue";
import Slider from "../core/slider.vue"
export default {
    components:{
        Panel,
        Slider
    },
    data(){
        return{
            items:[
                {
                    id:1,
                    href:"home",
                    src:"//img12.360buyimg.com/jrpmobile/jfs/t23905/169/686105059/44719/827e38a0/5b3df88aNe86eea3f.png"
                },
                  {
                    id:2,
                    href:"home",
                    src:"//img12.360buyimg.com/jrpmobile/jfs/t22225/196/1907552521/24475/fb4205ce/5b3df8cfN6e5c273d.jpg"
                },
                  {
                    id:3,
                    href:"home",
                    src:"//img12.360buyimg.com/jrpmobile/jfs/t21718/97/1954029010/46734/8cb0c56e/5b3df8a5N9b741c77.jpg"
                }
            ]
        }
    }
}
</script>

<style lang="scss" module>
    @import "../../css/element.scss";
    .panel{
        @include panel;
        >h4{
            display: none;
        }
        .content{
            .slider{
                margin-top: 120px;
            }
        }
    }  
  
</style>
