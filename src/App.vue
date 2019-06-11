<template>
<div id="app">
    <product-list-one v-bind:products="products"></product-list-one>
    <product-list-two v-bind:products="products"></product-list-two>
</div>
</template>

<script>
import ProductListOne from './components/ProductListOne.vue'
import ProductListTwo from './components/ProductListTwo.vue'

export default {
    name: 'app',
    components: {
        'product-list-one': ProductListOne,
        'product-list-two': ProductListTwo
    },
    data () {
        return {
            products: [
                {name: '鼠标', price: 20},
                {name: '键盘', price: 40},
                {name: '耳机', price: 60},
                {name: '显示屏', price: 80}
            ]
        }
    }
}
</script>

<style>
body{
    font-family: Ubuntu;
    color: #555;
}
</style>

作者：李棠辉
链接：https://www.jianshu.com/p/a804606ad8e9
来源：简书
简书著作权归作者所有，任何形式的转载都请联系作者获得授权并注明出处。