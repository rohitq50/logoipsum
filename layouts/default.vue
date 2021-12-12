<template>
	<div class="container">
		<Header />
		<Nuxt />
	</div>
</template>

<style lang="scss">
.color-yellow{
	&:hover {
		color: rgb(255, 194, 25);
	}
	color: rgb(255, 194, 25);
}
.color-red{
	&:hover {
		color: rgb(248, 41, 41);
	}
	color: rgb(248, 41, 41);
}
.color-brown {
	&:hover {
		color: rgb(180, 165, 144);
	}
	color: rgb(180, 165, 144);
}
.color-blue {
	&:hover {
		color: rgb(129, 126, 190);
	}
	color: rgb(129, 126, 190);
}
.main-button-0, .card-0 {
	color: white;
	background-color: rgb(255, 194, 25);
	border-color: rgb(255, 194, 25);
}
.main-button-1, .card-1 {
	color: white;
	background-color: rgb(248, 41, 41);
	border-color: rgb(248, 41, 41);
}
.main-button-2, .card-2 {
	color: white;
	background-color: rgb(180, 165, 144);
	border-color: rgb(180, 165, 144);
}
.main-button-3, .card-3 {
	color: white;
	background-color: rgb(129, 126, 190);
	border-color: rgb(129, 126, 190);
}

</style>