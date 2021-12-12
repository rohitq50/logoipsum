<template>
	<div class="card">
		<div class="card-body" :class="item.mainButtonCardClass">
			<div class="card-item d-flex">
				<div>
					<img :src="item.imageUrl" width="100" height="100">
				</div>
				<div>
					<p class="card-text">{{item.description}}</p>
					<div class="d-flex flex-row-reverse">
						<Button :classes="[item.titleBtnClass, 'btn btn-light btn-md']" />
					</div>
				</div>
			</div>
		</div>
	</div>
</template>
<script>
export default {
	props: ["item", "classes"]
}
</script>
<style lang="scss" scoped>
</style>