<template>
	<div class="footer">
			{{footerText}}
	</div>
</template>

<script>
export default {
  name: "homeneFooter",
  props:['footerText']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
	.footer {
		text-align:center;
		margin-bottom:10px;
	}
</style>
