<template>
  <div class="nav-bar">
    <div class="left">
      <slot name="left"></slot>
    </div>
    <div class="center">
      <slot name="center"></slot>
    </div>
    <div class="right">
      <slot name="right"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar"
};
</script>

<style scoped>
.nav-bar {
  display: flex;
  line-height: 44px; /**导航栏高度一般都是44px,状态栏20px,加在一起是64px;line-height:使文字自动上下居中 */
  box-shadow: 0 1px 1px rgba(100, 100, 100, 0.1);
}
.left,
.right {
  width: 60px;
  text-align: center;
}
.center {
  flex: 1;
  text-align: center;
}
</style>