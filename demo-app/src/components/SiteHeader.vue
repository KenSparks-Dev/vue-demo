<template>
<div class="site-header">
  <div class="site-header-content">
    <h1 class="site-title">{{title}}</h1>
    <nav>
      <ul class="pages">
        <li v-for="page in pages" :key="page.id">{{page.title}}</li>
      </ul>
    </nav>
  </div>
</div>
</template>
<script>
export default {
  name: 'SiteHeader',
  props: {
    title: String
  },
  data(){
    return{
      pages:[
        {
          id: 1,
          title: 'About',
          link: ''
        },
        {
          id: 2,
          title: 'Contact',
          link: ''
        }
      ]
    }
  }
}
</script>
<style scoped>
.site-header{
  background: #E0E0E0;
  }
.site-header-content{
  height: 100px;
  display:flex;
  align-items: center;
  justify-content: space-between;
  width: 85%;
  margin: 0 auto;
}
.site-title{
  padding-left: 10px;
}
.pages{
  display:grid;
  grid-template-columns: repeat(2, 1fr);
}
.pages li{
  list-style: none;
  width: 100%;
}
</style>