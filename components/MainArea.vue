<template>
	<div class="d-flex">
		<div class="p-5">
			<img :src="item.imageUrl" width="500" height="400">
		</div>
		<div class="right-block flex-grow-1 pt-5">
			<div class="product-heading pt-5">
				<Dot class="dot-postion"/>
				<div>{{item.title[0]}} <span :class="item.titleBtnClass">{{item.title[1]}}</span></div>
				<div>{{item.title[2]}}</div>
			</div>
			<div>
				<p>{{item.description}}</p>
			</div>
			<Button :classes="[item.mainButtonCardClass, 'btn btn-primary btn-lg']"/>
		</div>
	</div>
</template>
<script>
export default {
	props: ["item"]
}
</script>

<style lang="scss">
.right-block {
	.product-heading {
		position: relative;
		font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
		font-style: italic;
		font-weight: 600;
		font-size: 4rem;

		.dot-postion {
			position: absolute;
			top: 96px;
			right: 106px;
			width: 398px;
			height: 158px;
		}
		.yellow {
			color: rgb(255, 194, 25);
		}
	}
}

</style>