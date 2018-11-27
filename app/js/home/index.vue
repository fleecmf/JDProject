<template lang="html">
    <div>
        <JDHeader></JDHeader>
        <Slider></Slider>
        <Novice></Novice>
        <Borrow></Borrow>
        <Money></Money>
        <Product></Product>
        <Life></Life>
        <Footer></Footer>
        <Navbar></Navbar>
    </div>
</template>

<script>
import JDHeader from '../public/header'
import Footer from '../public/footer'
import Navbar from "../public/navbar.vue"
import Slider from './hslider.vue'
import Novice from './novice.vue'
import Borrow from './borrow.vue'
import Money from './money.vue'
import Product from './product.vue'
import Life from './life.vue'


export default {
  components: {
    JDHeader,
    Footer,
    Navbar,
    Slider,
    Novice,
    Borrow,
    Money,
    Product,
    Life
  },
}
</script>

<style lang="scss" module>
  @import '../../css/reset.scss';
</style>
