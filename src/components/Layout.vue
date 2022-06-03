<template>
    <div class="nav-wrapper">
    <div class="content">
     <slot/>
    </div>
    <Nav/>
  </div>
</template>

<script lang="ts">
    export default {
        name:'Layout'
    };
</script>

<style lang="scss" scoped>
.nav-wrapper{
      display: flex;
      flex-direction: column;
      height: 100vh;
  }
  .content{
      overflow: auto;
      flex-grow: 1;//在 flex 容器中分配剩余空间的相对比例，尽量把所有的高度都给content，nav占剩下的
  }
</style>