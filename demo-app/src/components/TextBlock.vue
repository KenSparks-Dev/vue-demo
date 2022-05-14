<template>
  <div class="text-block">
    <p>{{ text }}</p>
  </div>
</template>
<script>
export default {
  name: "TextBlock",
  props: {
    text: String,
  },
};
</script>
<style scoped>
.text-block {
  width: 90%;
  display: flex;
  margin-top: 20px;
}
@media (min-width: 768px) {
  .text-block {
    width: 60%;
    font-size: 1.2rem;
  }
}
</style>
