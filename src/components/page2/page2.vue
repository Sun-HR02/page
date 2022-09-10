<template>
<div>
    <div class="left"><page2-left></page2-left></div>
    <div class="right"><page2-right></page2-right></div>
</div>
  <div class="bottom">
<page2-bottom></page2-bottom>
</div>
</template>

<script>
import Page2Left from "@/components/page2/page2Left";
import Page2Right from "@/components/page2/page2Right";
import Page2Bottom from "@/components/page2/page2Bottom";
export default {
  name: "pageTwo",
  components: {Page2Bottom, Page2Right, Page2Left}
}
</script>

<style scoped>
.left{
  display: inline;
  position: fixed;
  left: 10%;
}
.right{
  display: inline;
  position: fixed;
  left: 50%;
}
.bottom{
  display: inline;
  position: fixed;
  bottom: 10%
}

</style>