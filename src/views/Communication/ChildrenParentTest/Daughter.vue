<template>
  <div style="background: #ccc; height: 50px">
    <h3>女儿小红: 有存款: {{ money }}</h3>
    <button @click="giveMoney(100)">给BABA钱: 100</button>
  </div>
</template>

<script>
// 引入myMixin.js
import myMixin from '@/views/Communication/ChildrenParentTest/myMixin/myMixin';
export default {
  name: 'Daughter',
  mixins: [myMixin],
  data() {
    return {
      money: 20000,
    };
  },
};
</script>
