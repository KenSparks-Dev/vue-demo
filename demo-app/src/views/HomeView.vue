<template>
  <div>
    <div class="content">
    <TextBlock text="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."/>
    <DemoList/>
    <TextBlock text="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur."/>
    </div>
  </div>
</template>

<script>
import TextBlock from '../components/TextBlock.vue';
import DemoList from '../components/DemoList.vue';
export default {
  name: 'HomePage',
  components: {
    TextBlock,
    DemoList
  }
}
</script>

<style>
.content{
  display:flex;
  align-items: center;
  flex-direction: column;
}
@media (min-width: 1024px) {
  .content{
    width: 70%;
    margin: 0 auto;
  }
}
</style>
