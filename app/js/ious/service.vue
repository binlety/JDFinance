<template lang="html">
      <Panel title="更多服务" :class="$style.panel">
                <section :class="$style.content">
                        <div  :class="$style.item" v-for="item in items" :key="item.src">
                                <img :src="item.src"/>
                                <p>{{item.text}}</p>
                        </div>
                </section>
        </Panel>
</template>

<script>
import Panel from "../core/panel.vue";
export default {
    components:{
        Panel
    },
    data(){
        return{
            items:[{
               src:"//img12.360buyimg.com/jrpmobile/jfs/t22912/282/79473391/6583/7174d493/5b247539N4854a034.png",
               text:"小白卡"
            },
            {
               src:"//img12.360buyimg.com/jrpmobile/jfs/t15922/204/1330308267/4745/e0cae4a0/5a4f2836Nd00354cb.png",
               text:"白条商城"
            },
            {
               src:"//img12.360buyimg.com/jrpmobile/jfs/t13051/63/2559290659/4702/e4068917/5a4f2693N937f1905.png",
               text:"消费分期"
            },
            {
               src:"//img12.360buyimg.com/jrpmobile/jfs/t14896/125/1435676873/3668/a8b392f7/5a4f26edN6cdfda66.png",
               text:"借钱"
            },
            {
               src:"//img12.360buyimg.com/jrpmobile/jfs/t20182/61/1301593180/9560/df0c6362/5b247663Nc83d2060.jpg",
               text:"白条提额"
            },
            {
               src:"//img12.360buyimg.com/jrpmobile/jfs/t12799/50/704102454/5247/19eac80a/5a4f2622Nc4aca701.png",
               text:"白条闪付"
            },
            {
               src:"//img12.360buyimg.com/jrpmobile/jfs/t15133/16/1440686097/5786/1b038e03/5a4f26bfN03ed1f66.png",
               text:"小白会玩"
            },
            {
               src:"//img12.360buyimg.com/jrpmobile/jfs/t16033/196/1306232362/4705/4c678227/5a4f265bN66ef5ae8.png",
               text:"钢镚"
            }]
        }
    }
}
</script>

<style lang="scss" module>
    @import "../../css/element.scss";
    .panel{
        @include panel;
        .content{
        @include flex(row);
            .item{
                width: 160px;
                height: 144px;
                text-align: center;
                  margin-bottom:40px; 
                img{
                    width: 90px;
                    height: 90px;
                }
                p{
                    font-size: 26px;
                    color: #666;
                    margin-top: 12px;
                }
            }
        }
    }
</style>
