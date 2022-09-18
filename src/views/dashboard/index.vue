<template>
  <div class="box">
    欢迎来到宿舍保修管理系统
    <!-- <Card></Card>
    <Sale></Sale>
    <Observe></Observe> -->
  </div>
</template>

<script>
import Sale from "./Sale";
import Card from "./Card";
import Observe from "./Observe";
export default {
  name: "",
  components: {
    Card,
    Sale,
    Observe,
  },
  mounted() {
    this.$store.dispatch("getData");
  },
};
</script>

<style scoped>
.box {
  font-size: 20px;
  margin: 30px;
}
</style>
