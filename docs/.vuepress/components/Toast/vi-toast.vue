<template>
    <div class="vi-layout">
      <div class="toast test">
        <button @click="showToast">点击</button>
        <button @click="showToast1">点击</button>
        <button @click="showToast2">点击</button>
    </div>
    </div>
</template>

<script>
import Vue from 'vue'
import ToastPlugin from '../../../../src/packages/toast/src/ToastPlugin.js'
Vue.use(ToastPlugin)

export default {
  components:{
  },
  methods: {
    showToast(){
      this.$toast({
        message:'提示信息',
        icon:{'name':'error','size':"small"},
        autoClose:false
      })
    },
    showToast1(){
      this.$toast({
        message:'提示信息',
        icon:{'name':'error','size':"small"},
        position: 'middle',
        autoClose:false
      })
    },
    showToast2(){     
      this.$toast({
        message:'提示信息',
        icon:{'name':'error',size:'small'},
        autoClose:false,
        position: 'bottom'
      })
    }
  }
}
</script>
<style scoped>
  hr{
    border:none;
  }
</style>