<template lang="html">
      <Panel title="每时专享" :class="$style.panel">
                <section :class="$style.content">
                      <img src="https://img12.360buyimg.com/jrpmobile/jfs/t20746/93/1719082958/12040/306a2296/5b31b40dNeefe4c3c.png"/>
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
            display: none;
        }
        .content{
             padding: 20px 0;
            img{
                display: block;
                width: 100%;
            }
        }
    }
</style>
