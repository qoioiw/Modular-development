<template>
  <div class="index">
    <div class="window">
      <div class="title">ApiKid</div>
      <div class="login-window">
        <LoginWindow />
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref, onMounted } from 'vue'
import LoginWindow from '@/components/login/LoginWindow.vue'
</script>

<style scoped lang="scss">
.index {
  width: 100%;
  height: 100vh;
  background: linear-gradient(180deg, #7c7c7c 0%, rgba(245, 245, 245, 0) 100%);

  .window {
    position: absolute;
    left: 65%;
    top: 50%;
    transform: translate(0, -55%);
    width: 400px;

    .title {
      font-family: 'Cursive', cursive;
      /* 使用手写风格字体，可以根据需要更换字体 */
      font-style: italic;
      /* 将文字设置为斜体 */
      font-size: 36px;
      /* 字体大小 */
      font-weight: bold;
      /* 字体粗细 */
      color: #280f09;
      /* 字体颜色，可以根据需要更改 */
      text-align: center;
      /* 文本居中对齐 */
      text-transform: uppercase;
      /* 文本转换为大写 */
      letter-spacing: 4px;
      /* 字母间距 */
      margin-bottom: 20px;
      /* 底部外边距 */
    }

    .login-window {
      background: linear-gradient(
        180deg,
        #7c7c7c 0%,
        rgba(245, 245, 245, 0) 100%
      );
    }
  }
}
</style>
