<template lang="html">
    <div>
        <Heador></Heador>
        <Hslider></Hslider>
        <Ada></Ada>
        <Money></Money>
        <Abd></Abd>
        <Finance></Finance>
       <Abc></Abc>
        <Footer cname="mfooter"></Footer>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header.vue"
import Footer from "../public/footer.vue"
import Navbar from "../public/navbar.vue"
import Money from "../home/money.vue"
import Hslider from "./mslider.vue"
import Ada from "./ada.vue"
import Abd from "./abd.vue"
import Finance from "./finance.vue"
import Abc from "./abc.vue"
export default {
    components:{
      Heador,
      Footer,
      Navbar,
      Hslider,
      Ada,
      Money,
      Abd,
      Finance,
     Abc
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
