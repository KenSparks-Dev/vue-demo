<template>
  <div class="profile-section">
    <TextBlockVue
      text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem error, nihil quod autem omnis, laboriosam obcaecati reiciendis ex voluptatum sunt nobis veritatis voluptates mollitia cupiditate dolores. Quidem consequuntur repellat iste. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem error, nihil quod autem omnis, laboriosam obcaecati reiciendis ex voluptatum sunt nobis veritatis voluptates mollitia cupiditate dolores. Quidem consequuntur repellat iste."
    />
    <img :src="imgSrc" :alt="imgAlt" />
  </div>
</template>

<script>
import TextBlockVue from "./TextBlock.vue";
export default {
  name: "ProfileSection",
  components: {
    TextBlockVue,
  },
  props: {
    text: String,
    imgSrc: String,
    imgAlt: String,
  },
};
</script>
<style scoped>
.profile-section {
  display: grid;
  grid-template-columns: 1fr 1fr;
  width: 90%;
  margin: 0 auto;
  margin-top: 2rem;
}
img {
  width: 100%;
  height: 400px;
  object-fit: cover;
}
.text-block {
  width: 90%;
}
</style>
