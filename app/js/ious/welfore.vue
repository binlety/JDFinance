<template lang="html">
      <Panel title="白条福利" :class="$style.panel">
                <section :class="$style.content">
                        <div  :class="$style.item">
                            <img src="https://img12.360buyimg.com/jrpmobile/jfs/t9739/355/2223965438/3092/b3cc4062/59f2fef3Nc2363e64.png"/>
                            <div>
                                    <h4>开通白条</h4>
                                    <p>送188元礼包</p>
                            </div>
                            <em>立即开通 ></em>
                        </div>
                         <div  :class="$style.item">
                            <img src="https://img12.360buyimg.com/jrpmobile/jfs/t10882/187/2325566882/2968/e64c911c/59f2ff2cNd85eb522.png"/>
                            <div>
                                    <h4>白条闪付</h4>
                                    <p>新手享158元礼包</p>
                            </div>
                            <em>随机立减 ></em>
                        </div>
                         <div  :class="$style.item">
                            <img src="https://img12.360buyimg.com/jrpmobile/jfs/t9523/348/2258037555/2792/9e8e1a80/59f2ff9fNf9648450.png"/>
                            <div>
                                    <h4>白条提额</h4>
                                    <p>金融app专享提额礼包</p>
                            </div>
                            <em>去提额 ></em>
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
                    width: 304px;
                    p{
                        color:#999;
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
