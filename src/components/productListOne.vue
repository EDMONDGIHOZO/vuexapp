<template>
  <div id="product-list-one">
    <h1>Products list | 1</h1>
    <ul>
      <li v-for="product in products" v-bind:key="product.price">
        <span class="name">{{product.name}}</span>
        <br>
        <span class="price">{{product.price}}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line no-undef
  props: ['products'],
  data() {
    return {};
  }
};
</script>
<style>
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