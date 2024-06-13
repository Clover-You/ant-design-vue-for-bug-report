<script setup lang="ts">
import { DatePicker, InputNumber } from 'ant-design-vue'
</script>

<template>
  <div>
    <p>1. 点击 DatePicker</p>
    <p>2. 点击页脚中的 InputNumber 并随便输入点内容</p>
    <p>3. 如果你点击 InputNumber 的 Control, 你会发现 DatePicker 立刻关闭</p>

    <DatePicker>
      <template #renderExtraFooter>
        <InputNumber style="width: 100%" placeholder="输入点内容" />
      </template>
    </DatePicker>
  </div>
</template>
