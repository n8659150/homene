<template>
  		<section :id='anchorTarget1'>

			<div class="container">
				<div class="row">

					<div class="col-md-offset-1 col-md-2 col-sm-3">
						<img :src="profileImg" class="wow fadeInUp img-responsive img-circle" data-wow-delay="0.2s" alt="about image">
					</div>

					<div class="col-md-8 col-sm-8">
						<h1 class="wow fadeInUp" data-wow-delay="0.6s">{{description}}</h1>
						<a href="#" class="wow fadeInUp btn btn-default section-btn" data-wow-delay="1s">Download Resume</a>
					</div>

				</div>
			</div>
		</section>
</template>

<script>
export default {
  name: "homeneHome",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
	},
	props:['anchorTarget1','profileImg','description']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
