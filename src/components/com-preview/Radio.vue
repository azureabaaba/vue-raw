<template>
  <div>
    <!-- 单选 -->
    <span>单选框radio：</span>
    <el-radio v-model="radioValue" value="1">单选1</el-radio>
    <el-radio v-model="radioValue" value="2">单选2</el-radio>
    <span>按钮样式</span>
    <el-radio-group v-model="radioGroup">
        <el-radio-button value="上海">shanghai</el-radio-button>
      <el-radio-button value="北京">beijing</el-radio-button>
      <el-radio-button value="广州">guangzhou</el-radio-button>
      <el-radio-button value="深圳">shenzhen</el-radio-button>
    </el-radio-group>
  </div>
</template>

<script lang="ts" setup>
import { ref, onMounted } from "vue";

const radioValue = ref("1");
const radioGroup = ref('北京')
</script>

<style lang="less" scoped></style>
