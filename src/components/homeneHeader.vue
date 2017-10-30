<template>
  		<div class="navbar custom-navbar navbar-fixed-top" role="navigation">
			<div class="container">

				<div class="navbar-header">
					<button class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse">
                    <span class="icon icon-bar"></span>
                    <span class="icon icon-bar"></span>
                    <span class="icon icon-bar"></span>
               </button>
					<!-- lOGO TEXT HERE -->
					<a href="index.html" class="navbar-brand">{{siteTitle}}</a>
				</div>

				<div class="collapse navbar-collapse">
					<ul class="nav navbar-nav navbar-right">
						<li><a class="smoothScroll" :href="'#' + anchorMapping1">{{navItem1}}</a></li>
						<li><a class="smoothScroll" :href="'#' + anchorMapping2">{{navItem2}}</a></li>
						<li><a class="smoothScroll" :href="'#' + anchorMapping3">{{navItem3}}</a></li>
						<li><a class="smoothScroll" :href="'#' + anchorMapping4">{{navItem4}}</a></li>
					</ul>
				</div>

			</div>
		</div>
</template>

<script>
export default {
  name: "homeneHeader",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
	},
	props:['siteTitle','navItem1','navItem2','navItem3','navItem4','anchorMapping1','anchorMapping2','anchorMapping3','anchorMapping4']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
