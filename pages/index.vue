<template>
	<div>
		<MainArea
			:item="items[selectedItem]"
		/>
		<div class="d-flex justify-content-between">
			<div  v-for="(item, i) in items" :key="i" @click="selectedItem = i">
				<CardItem
					v-if="i != selectedItem"
					class="mx-3"
					:item="item"
				/>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			selectedItem: 0,
			items: [
				{
					title: ["New", "Winter", "Arrivals"],
					title2: ["Buy", "Women Shoe", "Now"],
					imageUrl: "shoe.png",
					titleBtnClass: "color-yellow",
					mainButtonCardClass: "card-0",
					description: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. voluptatum totam? Distinctio itaque non iure aut illo illum autem."
				},
				{
					title: ["New", "Winter", "Arrivals"],
					title2: ["Buy", "Women Shoe", "Now"],
					imageUrl: "1-shoe.png",
					titleBtnClass: "color-red",
					mainButtonCardClass: "card-1",
					description: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. voluptatum totam? Distinctio itaque non iure aut illo illum autem."
				},
				{
					title: ["New", "Winter", "Arrivals"],
					title2: ["Buy", "Women Shoe", "Now"],
					imageUrl: "2-shoe.png",
					titleBtnClass: "color-brown",
					mainButtonCardClass: "card-2",
					description: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. voluptatum totam? Distinctio itaque non iure aut illo illum autem."
				},
				{
					title: ["New", "Winter", "Arrivals"],
					title2: ["Buy", "Women Shoe", "Now"],
					imageUrl: "3-shoe.png",
					titleBtnClass: "color-blue",
					mainButtonCardClass: "card-3",
					description: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. voluptatum totam? Distinctio itaque non iure aut illo illum autem."
				}
			]
		}
	}
}
</script>
