<template>
  <div class="about">
   <ProfileSectionVue imgSrc="https://cdn.vox-cdn.com/thumbor/q-2sSjgnbVgJnqULYyfEf2JL8Xo=/0x0:915x610/1200x800/filters:focal(377x20:523x166)/cdn.vox-cdn.com/uploads/chorus_image/image/58796435/boseman.0.jpg" imgAlt="logo" text="lorem" />
  </div>
</template>
<script>
import ProfileSectionVue from "@/components/ProfileSection.vue"
export default{
  name: "AboutView",
  components: {
    ProfileSectionVue,
  }
}
</script>