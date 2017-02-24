<template>
	<div id="contain">
		<home-header></home-header>
		<div class="content">
			<ul class="con_ul">
				<list 
					v-for="(item,inx) in items"
					:price="item.price"
					:title="item.title"
					:index="inx"
				></list>
			</ul>
		</div>
	</div>
</template>
<script type="text/javascript">
	import HomeHeader from '../components/HomeHeader'
	import List from '../components/List'
	export default {
		data(){
			return {
				items:[
						{ price: "129.00", title: "大学" },  
	                    { price: "256.00", title: "中庸" },  
	                    { price: "399.00", title: "论语" },  
	                    { price: "998.00", title: "孟子" },  
	                    { price: "99.00", title: "道德经" },  
	                    { price: "89.00", title: "老子" },  
	                    { price: "188.00", title: "金刚经" },  
	                    { price: "209.00", title: "易筋经" }  
				]
			}
		},
		components:{
				HomeHeader,
				List
		}
	}
</script>
<style type="text/css">
	.con_ul{
		margin-top:5.5rem;
	}
</style>