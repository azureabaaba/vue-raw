<template>
  <div>
    <span>多选框checkbox</span>
    <el-checkbox v-model="checkedSingle">单个多选</el-checkbox>
    <span>多选框组checkbox group</span>
    <el-checkbox-group v-model="checkList" @input="(v)=>console.log(v)">
      <el-checkbox label="复选框 A"></el-checkbox>
      <el-checkbox label="复选框 B"></el-checkbox>
      <el-checkbox label="复选框 C"></el-checkbox>
      <el-checkbox label="禁用" disabled></el-checkbox>
      <el-checkbox label="选中且禁用" disabled></el-checkbox>
    </el-checkbox-group>
  </div>
</template>

<script lang="ts" setup>
import { ref, onMounted } from "vue";

defineProps({
  msg: String,
});
const checkedSingle = ref(false);
const checkList = ref(['选中且禁用']);
const fn = () => {};
onMounted(() => {});
</script>

<style lang="less" scoped></style>
