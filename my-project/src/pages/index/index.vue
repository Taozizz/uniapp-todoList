<template>
	<view>
		<text>This is a {{ product_name }}</text>
		<button @click.prevent="handleClick">BUTTON</button>
	</view>

</template>

<script>
	export default{
		data(){
			return {
				product_name: 'Todo List'
			}
		},
		methods: {
			handleClick() {
				this.product_name += '!'
			}
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin: 200rpx auto 50rpx auto;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
