<template>
  <div class="directory">
    <div class="name">
      <slot name="name"></slot>
    </div>
    <div class="description">
      <slot name="description"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "BlogDirectory",
};
</script>

<style scoped>
.directory {
  box-sizing: border-box;
  width: 280px;
  margin: 10px;
  padding: 16px;
  border-radius: 3px;
  box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2);
  font-family: var(--text-font);
  cursor: pointer;
}

.name {
  margin-bottom: 10px;
  height: 30px;
  line-height: 30px;

  text-align: left;
  font-size: 16px;
  color: #0366d6;

  white-space: nowrap; /* 先强制一行内显示文本 */
  overflow: hidden; /* 超出部分隐藏 */
  text-overflow: ellipsis; /* 文字用省略号代替超出的部分 */
}
.description {
  font-size: 14px;
  color: #586069;
  line-height: 1.8;
}
</style>
