<template>
	<div class="b-body">
		<ul class="vidbox v-list">
			<BRowItem v-for="item in row" :item="item" :key="item"></BRowItem>
		</ul>
	</div>
</template>

<script>
import BRowItem from 'components/contentRow/BRowItem'
export default {
	props: {
		row: {
			type: Array
		}
	},
	components: {
		BRowItem
	}
}
</script>

<style lang="styl" scoped>
	.b-body
		margin-right -20px
		clear both
		.v-list
			width 100%
			height 316px
			overflow hidden
			padding-top 20px
</style>