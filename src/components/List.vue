<template>
	<li class="sec_li">
		<router-link :to="{name:'detail',params:{id:index}}">
			<div class="lp_li_img">
				<img src="../assets/img/lp_01.jpg">
			</div>
			<div class="lp_li_name">《{{title}}》</div>
			<div class="lp_li_price">￥{{price}}</div>
		</router-link>
	</li>
</template>
<script type="text/javascript">
	export default {
		name:"detail",
		template:"<List/>",
		props:['title','price','index']
	}
</script>
<style type="text/css">
	.sec_li{
		width:49%;
		float: left;
		background: #FFF;
		list-style: none;
		margin-bottom:0.6rem; 
		box-shadow: 0.1rem 0.1rem 1rem #AAA;
	}
	.sec_li:nth-of-type(even){
		float: right;
	}
	.lp_li_img{
		width: 100%;
		height: 70%;
		text-align: center;
	}
	.lp_li_img img{
		width: 80%;
		height: 80%;
		margin-top: 5%;
	}
	.lp_li_name{
		width: 100%;
		font-size: 2rem;
		margin-top: 2%;
		text-align: center;
		color:#000;
	}
	.lp_li_price{
		width: 100%;
		font-size: 1.5rem;
		margin-top: 2%;
		color:deeppink;
		text-align: center;
		font-weight:bold;
		margin-bottom:2%;
	}
</style>