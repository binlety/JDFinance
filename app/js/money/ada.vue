<template lang="html">
      <Panel title="神券满" :class="$style.panel">
                <section :class="$style.content">
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t22375/348/1946619980/53612/5abf594/5b3dfb59N84b22aab.jpg"/>
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
            img{
                display: block;
                width: 100%;
            }
        }
    }
</style>
