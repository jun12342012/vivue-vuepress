<template>
  <div>
    <vi-row class="row-bg">
      <vi-col :span="6"><div class="grid-content bg-purple"></div></vi-col>
      <vi-col :span="6"><div class="grid-content bg-purple-light"></div></vi-col>
      <vi-col :span="6"><div class="grid-content bg-purple"></div></vi-col>
    </vi-row>
    <vi-row class="row-bg" justify="center">
      <vi-col :span="6"><div class="grid-content bg-purple"></div></vi-col>
      <vi-col :span="6"><div class="grid-content bg-purple-light"></div></vi-col>
      <vi-col :span="6"><div class="grid-content bg-purple"></div></vi-col>
    </vi-row>
    <vi-row class="row-bg" justify="end">
      <vi-col :span="6"><div class="grid-content bg-purple"></div></vi-col>
      <vi-col :span="6"><div class="grid-content bg-purple-light"></div></vi-col>
      <vi-col :span="6"><div class="grid-content bg-purple"></div></vi-col>
    </vi-row>
    <vi-row class="row-bg" justify="between">
      <vi-col :span="6"><div class="grid-content bg-purple"></div></vi-col>
      <vi-col :span="6"><div class="grid-content bg-purple-light"></div></vi-col>
      <vi-col :span="6"><div class="grid-content bg-purple"></div></vi-col>
    </vi-row>
    <vi-row class="row-bg" justify="around">
      <vi-col :span="6"><div class="grid-content bg-purple"></div></vi-col>
      <vi-col :span="6"><div class="grid-content bg-purple-light"></div></vi-col>
      <vi-col :span="6"><div class="grid-content bg-purple"></div></vi-col>
    </vi-row>
  </div>
</template>

<script>
import Col from '../../../../src/packages/grid/src/col'
import Row from '../../../../src/packages/grid/src/row'
export default {
  components:{
    viCol: Col,
    viRow: Row
  }
}
</script>
<style lang="scss" scoped>
  .vi-row {
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .vi-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: #7aa9bf;
  }
  .bg-purple {
    background: #badce6;
  }
  .bg-purple-light {
    background: #cce9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
</style>