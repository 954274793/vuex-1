<template>
    <div id="product-list-one">
        <h2>Product List One</h2>
        <ul>
            <li v-for="product in products">
                <span class="name">{{ product.name }}</span>
                <span class="price">${{ product.price }}</span>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    data () {
        return {
            products : this.$store.state.products //获取store中state的数据
        }
    }
}
</script>

<style scoped>
#product-list-one{
    background: #FFF8B1;
    box-shadow: 1px 2px 3px rgba(0,0,0,0.2);
    margin-bottom: 30px;
    padding: 10px 20px;
}
#product-list-one ul{
    padding: 0;
}
#product-list-one li{
    display: inline-block;
    margin-right: 10px;
    margin-top: 10px;
    padding: 20px;
    background: rgba(255,255,255,0.7);
}
.price{
    font-weight: bold;
    color: #E8800C;
}
</style>

作者：李棠辉
链接：https://www.jianshu.com/p/a804606ad8e9
来源：简书
简书著作权归作者所有，任何形式的转载都请联系作者获得授权并注明出处。