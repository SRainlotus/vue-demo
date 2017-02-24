<template>
	<div class="detail_pane">
		<div class="img_wrap">
			<img src="../assets/img/lp_01.jpg">
		</div>
		<div class="discrip">
			<p>{{first}}</p>
			<p>{{second}}</p>
			<p>{{u}}</p>
		</div>
	</div>
</template>
<script type="text/javascript">
	export default {
		template:"<DetailContent/>",
		props:["first","second","u"]
	}
</script>
<style type="text/css">
	.img_wrap{
		width:100%;
		text-align:center;
		padding-top: 3rem;
	}
	.detail_pane{
		background:#FFF;
		width: 100%;
		height: 100%;
		font-size:1.5rem;
	}
	.content p{
		padding: 1rem;
		text-indent: 2.5rem;
		line-height: 2rem;
		margin: 0;
	}
</style>
