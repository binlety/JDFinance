<template lang="html">
    <div>
        <Heador></Heador>
        <Slider></Slider>
        <Daily></Daily>
        <In></In>
        <More></More>
        <Footer cname="mfooter"></Footer>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header.vue"
import Footer from "../public/footer.vue"
import Navbar from "../public/navbar.vue"
import Slider from "./rslider.vue"
import Daily from "./daily.vue"
import In from "./in.vue"
import More from "./more.vue"
export default {
    components:{
      Heador,
      Footer,
      Navbar,
      Slider,
      Daily,
      In,
      More
    }
}
</script>

<style lang="scss">
    .mfooter{
        margin-top: 0;
       ul{
           li:first-child{
               display: none;
           }
       }
    }
</style>

