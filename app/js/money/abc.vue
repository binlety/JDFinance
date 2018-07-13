<template lang="html">
      <Panel title="京东智投" :class="$style.panel">
                <section :class="$style.content">
                      <img src="https://img12.360buyimg.com/jrpmobile/jfs/t19756/137/1902911799/17823/e19ffe7b/5add9511Nf6984e89.jpg"/>
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
        margin-bottom: 0;
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
