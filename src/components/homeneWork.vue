<template>
  		<section :id="anchorTarget3">
			<div class="container">
				<div class="row">

					<div class="col-md-12 col-sm-12">
						<div class="wow fadeInUp section-title" data-wow-delay="0.2s">
							<h2>Seleted Works</h2>
							<p>Lorem ipsum dolor sit amet, consectetur venenatis tincidunt.</p>
						</div>
					</div>

					<div class="wow fadeInUp col-md-3 col-sm-6" data-wow-delay="0.4s">
						<!-- WORK THUMB -->
						<div class="work-thumb">
							<a href="../../static/images/work-1.jpg" class="image-popup">
								<img src="../../static/images/work-1.jpg" class="img-responsive" alt="Work">
							</a>
						</div>
						<h4>Graphic & Branding</h4>
					</div>

					<div class="wow fadeInUp col-md-3 col-sm-6" data-wow-delay="0.6s">
						<!-- WORK THUMB -->
						<div class="work-thumb">
							<a href="../../static/images/work-2.jpg" class="image-popup">
								<img src="../../static/images/work-2.jpg" class="img-responsive" alt="Work">
							</a>
						</div>
						<h4>Logo Design</h4>
					</div>

					<div class="wow fadeInUp col-md-3 col-sm-6" data-wow-delay="0.8s">
						<!-- WORK THUMB -->
						<div class="work-thumb">
							<a href="../../static/images/work-3.jpg" class="image-popup">
								<img src="../../static/images/work-3.jpg" class="img-responsive" alt="Work">
							</a>
						</div>
						<h4>Photography</h4>
					</div>

					<div class="wow fadeInUp col-md-3 col-sm-6" data-wow-delay="0.8s">
						<!-- WORK THUMB -->
						<div class="work-thumb">
							<a href="../../static/images/work-4.jpg" class="image-popup">
								<img src="../../static/images/work-4.jpg" class="img-responsive" alt="Work">
							</a>
						</div>
						<h4>Minimal Themes</h4>
					</div>

				</div>
			</div>
		</section>
</template>

<script>
export default {
  name: "homeneWork",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
	},
	props:['anchorTarget3']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
