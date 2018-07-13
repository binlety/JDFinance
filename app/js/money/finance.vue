<template lang="html">
      <Panel title="理财精选" :class="$style.panel">
                <section :class="$style.content">
                        <div  :class="$style.item">
                            <img src="https://img12.360buyimg.com/jrpmobile/jfs/t8929/33/1393593833/1749/1e115bd7/59b900e6N73c7b311.png"/>
                            <div>
                                    <h4>月度理财</h4>
                                    <p>预期年化收益率4.50%</p>
                            </div>
                            <em>去赚钱 ></em>
                        </div>
                         <div  :class="$style.item">
                            <img src="https://img12.360buyimg.com/jrpmobile/jfs/t9040/57/2313007861/3024/82c36c44/59ca556eNb605e901.png"/>
                            <div>
                                    <h4>季度理财</h4>
                                    <p>历史年化收益率5.50%</p>
                            </div>
                            <em>去赚钱 ></em>
                        </div>
                         <div  :class="$style.item">
                            <img src="https://img12.360buyimg.com/jrpmobile/jfs/t8902/275/1411242449/2807/a2cc902a/59b90111N4e88098c.png"/>
                            <div>
                                    <h4>一年理财</h4>
                                    <p>预期年化收益率5.80%</p>
                            </div>
                            <em>去赚钱 ></em>
                        </div>
                </section>
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
        >h4{
            border-bottom: 1px solid #ddd;
        }
        .content{
            @include flex;
           .item{
                @include flex(row);
                align-items: center;
                vertical-align: middle;
                height: 140px;
                &:after{
                    content:"";
                    box-sizing: border-box;
                    height: 0;
                    width: 100%;
                    border-bottom: 1px solid #ddd;
                    margin-left: 140px;
                }
                &:last-child:after{
                    border-bottom-color: #fff;
                }
                >img{
                    height:68px;
                    width:68px;
                    display:inline-block;
                    margin:0 32px;
                }
                >div{
                    font-size:32px;
                    color:#333;
                    line-height:1.8;
                    width: 344px;
                    p{
                        color:#ff3232;
                        font-size:24px;
                        line-height:1.1;
                        white-space: nowrap;
                        text-overflow: ellipsis;
                        overflow: hidden;
                    }
                }
                >em{
                    color: #FF801A;
                    font-size: 28px;
                }
           }
        }
    }
</style>
