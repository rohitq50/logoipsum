<template>
	<div class="navbar-expand-lg">
		<div class="container-fluid">
			<div class="d-flex justify-content-between">
				<div class="p-1 logo" @click="isActive = 0">
					<Logoipsum />
				</div>
				<ul class="navbar-nav">
					<li class="pe-2 nav-item">
						<div :class="['p-2', activeRoute == '/' ? activeClass : '']" @click="changeRoutes('/')">HOME</div>
					</li>
					<li class="ps-2 nav-item">
						<div :class="['p-2', activeRoute == '/buy' ? activeClass : '']" @click="changeRoutes('/buy')">BUY</div>
					</li>
				</ul>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			activeRoute: "/",
			activeClass: "active"
		}
	},
	methods: {
		changeRoutes(route) {
			this.activeRoute = route
			this.$router.push(route)
		}
	}
}
</script>

<style lang="scss" scoped>
.logo{
	cursor: pointer;
}
.nav-item {
	color: black;
	cursor: pointer;
	.active {
		border-bottom: 2px solid black;
	}
}
</style>
