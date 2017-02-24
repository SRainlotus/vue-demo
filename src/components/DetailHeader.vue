<template>
	<div class="header">
		<router-link to="/" class="back">
			<span>返回</span>
		</router-link>
		<div class="header_inner">详情页面</div>
	</div>
</template>
<style type="text/css">
	.header{
		width: 100%;
		height:5rem;
		background: #FFF;
		margin-bottom: 0.5rem;
		box-shadow: 0.2rem 0 1rem #000;
		position:fixed;
		top: 0;
	}
	.header_inner{
		width: 100%;
		height:100%;
		font-size: 2rem;
		font-weight:bold;
		text-align: center;
		line-height: 5rem;
	}
	.back{
		font-size:1.4rem;
		position:absolute;
		color:#000;
		top:50%;
		margin-top:-0.7rem;
		left:0.5rem;
	}
</style>