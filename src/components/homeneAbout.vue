<template>
<section :id="anchorTarget2">
			<div class="container">
				<div class="row">

					<div class="col-md-8 col-sm-12">
						<div class="about-thumb">
							<div class="wow fadeInUp section-title" data-wow-delay="0.6s">
								<h2>A Little Bit Of My Story</h2>
								<p><strong>Senior Interactive Designer & Web Developer at yourdreamjob.com</strong></p>
							</div>
							<div class="wow fadeInUp" data-wow-delay="0.8s">
								<p>Award winning interdisciplinary Designer & Art director. We have a team who specialise in coding websites and themes
									perfect blend of style and function for a wide range of interactive product design.</p>
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
							<a href="https://www.instagram.com/p/cqED9yjN0j/">
								<img :src="image1" class="img-responsive" alt="instagram image">
							</a>

							<a href="https://www.instagram.com/p/enL0SsDN51/">
								<img :src="image2" class="img-responsive" alt="instagram image">
							</a>

							<a href="https://www.instagram.com/p/apOuRTDNwJ/">
								<img :src="image3" class="img-responsive" alt="instagram image">
							</a>

							<a href="https://www.instagram.com/p/ZXIj33jN2v/">
								<img :src="image4" class="img-responsive" alt="instagram image">
							</a>

							<a href="https://www.instagram.com/p/Xwev1FjN9-/">
								<img :src="image5" class="img-responsive" alt="instagram image">
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
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
	},
	props:['anchorTarget2','image1','image2','image3','image4','image5']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
