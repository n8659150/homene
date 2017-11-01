<template>
<section :id="anchorTarget2">
			<div class="container">
				<div class="row">

					<div class="col-md-8 col-sm-12">
						<div class="about-thumb">
							<div class="wow fadeInUp section-title" data-wow-delay="0.6s">
								<h2{{aboutTitle}}</h2>
								<p><strong>{{aboutIntro}}</strong></p>
							</div>
							<div class="wow fadeInUp" data-wow-delay="0.8s">
								<p>{{aboutParas}}</p>
							</div>
							<ul class="social-icon">
								<li class="wow fadeInLeft" data-wow-delay="1s">
									<a href="#" class="fa fa-twitter"></a>
								</li>
								<li class="wow fadeInUp" data-wow-delay="1.2s">
									<a href="#" class="fa fa-linkedin"></a>
								</li>
								<li class="wow fadeInRight" data-wow-delay="1.4s">
									<a href="#" class="fa fa-dribbble"></a>
								</li>
							</ul>
						</div>
					</div>

					<div class="col-md-4 col-sm-12">
						<div class="wow fadeInUp" data-wow-delay="0.4s">
							<h2>On Instagram</h2>
						</div>

						<div class="wow fadeInUp" data-wow-delay="0.6s">
							<a :href="image1Link">
								<img :src="image1" class="img-responsive" alt="profolio image">
							</a>

							<a :href="image2Link">
								<img :src="image2" class="img-responsive" alt="profolio image">
							</a>

							<a :href="image3Link">
								<img :src="image3" class="img-responsive" alt="profolio image">
							</a>

							<a :href="image4Link">
								<img :src="image4" class="img-responsive" alt="profolio image">
							</a>

							<a :href="image5Link">
								<img :src="image5" class="img-responsive" alt="profolio image">
							</a>
						</div>
					</div>

				</div>
			</div>
		</section>

</template>

<script>
export default {
  name: "homeneAbout",
  props:['anchorTarget2','aboutTitle','aboutIntro','aboutParas','image1','image1Link','image2','image2Link','image3','image3Link','image4','image4Link','image5','image5Link']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
