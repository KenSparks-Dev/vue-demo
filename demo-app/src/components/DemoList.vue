
<template>
<ul class="demo-list" id="demo-list">
<li v-for="item in items" :key="item.id">
  <button @click='selectedBtn' v-bind:id='item.id'>{{item.text}}</button>
</li>
</ul>
</template>
<script>
export default {
  name: 'DemoList',
  data() {
    return {
  items:[
  {
    id: 1,
    text: 'Item 1'
  },
   {
    id: 2,
    text: 'Item 2'
  }
 ]   
    }
  },
  methods: {
    selectedBtn(){
			const one = document.getElementById('1');
			const two = document.getElementById('2');
			
			one.addEventListener('click', () => {
				one.classList.add('active');
				two.classList.remove('active');
			});
			
			two.addEventListener('click', () => {
				two.classList.add('active');
				one.classList.remove('active');
			});
    }
  }
}
</script>
<style>
.demo-list{
  width: 40%;
  display: flex;
  margin-top: 20px;
}
ul{
  display:flex;
  list-style: none;
  justify-content: space-between;
  width: 100%;
}
button{
  border-radius: 50%;
  width: 60px;
  height: 60px;
}
.active {
	background: green;
	color: white;
}
</style>