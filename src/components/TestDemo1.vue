<template>
  <div>
    <button @click="add" class="btn">+1</button>
    <button @click="reduce" :disabled="curNum < 1" class="btn">-1</button>
    <span>当前数值：{{curNum}}</span>
  </div>
</template>
<script>
import {numAdd, NumRe} from 'xinzhichao-test';
export default {
  data() {
    return {
      curNum: 0,
    }
  },
  methods: {
    add() {
      this.curNum = numAdd(this.curNum);
    },
    reduce() {
      this.curNum = NumRe(this.curNum);
    }
  },
};
</script>
<style scoped>
.btn {
  width: 50px;
  height: 30px;
  margin-right: 10px;
}
</style>