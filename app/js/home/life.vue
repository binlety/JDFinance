<template lang="html">
        <Panel title="生活服务" :class="$style.panel">
                <ul :class="$style.content">
                    <li :class="$style.item">
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t12799/50/704102454/5247/19eac80a/5a4f2622Nc4aca701.png"/>
                        <p>惠加油</p>
                    </li>
                      <li :class="$style.item">
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t16033/196/1306232362/4705/4c678227/5a4f265bN66ef5ae8.png"/>
                        <p>小白信用</p>
                        <p>全新升级</p>
                    </li>
                      <li :class="$style.item">
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t13051/63/2559290659/4702/e4068917/5a4f2693N937f1905.png"/>
                        <p>信用卡还款</p>
                    </li>
                      <li :class="$style.item">
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t15133/16/1440686097/5786/1b038e03/5a4f26bfN03ed1f66.png"/>
                        <p>卡转让</p>
                    </li>
                      <li :class="$style.item">
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t14896/125/1435676873/3668/a8b392f7/5a4f26edN6cdfda66.png"/>
                        <p>定期还款</p>
                    </li>
                </ul>
        </Panel>
</template>

<script>
import Panel from "../core/panel.vue";
export default {
    components:{
        Panel
    }
}
</script>

<style lang="scss" module>
    @import "../../css/element.scss";
    .panel{
        @include panel;
        .content{
            @include flex(row);
            padding-bottom: 40px;
            box-sizing: border-box;
            .item{
                width: 20%;
                text-align: center;
                img{
                    width: 90px;
                    height: 90px;
                }
                p{
                    font-size: 26px;
                    color: #666;
                    text-overflow: ellipsis;
                    white-space: nowrap;
                    overflow: hidden;
                    margin-top: 12px;
                    &:nth-child(3){
                        color: #FF801A;
                    }
                }
            }
        }
    }  
  
</style>
