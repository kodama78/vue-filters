<template>
		<div>
			<h1>Filters & Mixins</h1>
			<hr>
			<input type="text" v-model="filterText">
			<ul>
				<li v-for="fruit in filteredFruits">{{ fruit }}</li>
			</ul>
		</div>
</template>

<script>
	import { fruitMixin } from './fruitMixin';
	export default {
		mixins: [fruitMixin]
	}
</script>

<style>

</style>
