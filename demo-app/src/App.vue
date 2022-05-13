<template>
  <div id="app">
    <SiteHeader title="Demo"/>
    <HomePage/>
    <AboutPage/>
  </div>
</template>

<script>
import SiteHeader from './components/SiteHeader';
import HomePage from './vues/HomePage';
import AboutPage from './vues/AboutPage';
export default {
  name: 'App',
  components: {
  SiteHeader,
   HomePage,
   AboutPage,
  }
}
</script>

<style>
#app {
font-family: 'Koulen', cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
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
