<template>
<div class="site-header">
<h1 class="site-title">{{title}}</h1>
</div>
</template>
<script>
export default {
  name: 'SiteHeader',
  props: {
    title: String
  }
}
</script>
<style scoped>
.site-header{
  height: 100px;
  background: #E0E0E0;
  display:flex;
  align-items: center;
}
.site-title{
  padding-left: 10px;
}
</style>