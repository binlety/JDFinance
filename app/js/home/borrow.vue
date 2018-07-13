<template lang="html">
      <Panel title="极速借贷" :class="$style.panel">
                <section :class="$style.content">
                    <router-link :to="{name:'home'}">
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t23095/339/640414013/48531/7d7396cf/5b39e732N85f572ea.jpg"/>
                    </router-link>
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
        .content{
            padding-bottom: 40px;
            a{
                margin: 0px;
            }
            img{
                display: block;
                width: 100%;
            }
        }
    }
</style>
