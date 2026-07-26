<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****2211 获得了微信刚加好友 3 句破冰开场白"
  },
  {
    "text": "用户 189****7744 得到了 5 句甜度超标的奶茶店约会情话"
  },
  {
    "text": "用户 131****3399 完成了被吐槽“你好油”的高情商解套说辞"
  },
  {
    "text": "用户 156****4400 生成了朋友圈趣味互动幽默点赞评论"
  },
  {
    "text": "用户 173****8855 取得了暧昧期拉近距离的情感升温指南"
  }
]);
</script>
