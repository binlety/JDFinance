<template lang="html">
    <div>
        <Heador></Heador>
        <Slider></Slider>
        <Welfore></Welfore>
        <Service></Service>
        <Footer></Footer>
        <Navbar></Navbar>
    </div>
</template>

<script>
import Heador from "../public/header.vue"
import Footer from "../public/footer.vue"
import Navbar from "../public/navbar.vue"
import Slider from "./islider.vue"
import Welfore from "./welfore.vue"
import Service from "./service.vue"
export default {
    components:{
      Heador,
      Footer,
      Navbar,
      Slider,
      Welfore,
      Service
    }
}
</script>

<style lang="scss">
</style>
