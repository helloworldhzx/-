<template>
  <div class='common-card'>
    <div class='title'>{{title}}</div>
    <div class='value'>{{value}}</div>
    <div class='card'>
      <slot></slot>
    </div>
    <div class='line' />
    <div class='total'>
      <slot name="total"></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    value: String
  }
}
</script>

<style lang='scss' scoped>
  .title {
    font-size: 12px;
    color: #999;
  }
  .value {
    font-size: 25px;
    color: #000;
    margin-top: 5px;
    letter-spacing: 1px;
  }
  .card {
    height: 50px;
  }
  .line {
    margin: 10px 0;
    border-top: 1px solid #eee;
  }
  .total {
    font-size: 12px;
    color: #666;
  }
</style>

<style>
  .emphasis {
    margin-left: 5px;
    color: #333;
    font-weight: 700;
  }
  .increase{
        display: inline-block;
        border: 3px solid transparent;
        border-bottom-color: red;
        margin: 0 0 3px 5px;
      }
  .decrease{
    display: inline-block;
    border: 3px solid transparent;
    border-top-color: green;
    margin: 3px 0 0 5px;
  }
</style>
