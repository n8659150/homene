<template>
  		<section :id="anchorTarget3">
			<div class="container">
				<div class="row">

					<div class="col-md-12 col-sm-12">
						<div class="wow fadeInUp section-title" data-wow-delay="0.2s">
							<h2>{{workTitle}}</h2>
							<p>{{workDesc}}</p>
						</div>
					</div>

					<div class="wow fadeInUp col-md-3 col-sm-6" data-wow-delay="0.4s">
						<!-- WORK THUMB -->
						<div class="work-thumb">
							<a :href="thumb1link" class="image-popup">
								<img :src="thumb1img" class="img-responsive" alt="Work">
							</a>
						</div>
						<h4>{{thumb1Title}}</h4>
					</div>

					<div class="wow fadeInUp col-md-3 col-sm-6" data-wow-delay="0.6s">
						<!-- WORK THUMB -->
						<div class="work-thumb">
							<a :href="thumb2link" class="image-popup">
								<img :src="thumb2img" class="img-responsive" alt="Work">
							</a>
						</div>
						<h4>{{thumb2Title}}</h4>
					</div>

					<div class="wow fadeInUp col-md-3 col-sm-6" data-wow-delay="0.8s">
						<!-- WORK THUMB -->
						<div class="work-thumb">
							<a :href="thumb3link" class="image-popup">
								<img :src="thumb3img" class="img-responsive" alt="Work">
							</a>
						</div>
						<h4>{{thumb3Title}}</h4>
					</div>

					<div class="wow fadeInUp col-md-3 col-sm-6" data-wow-delay="0.8s">
						<!-- WORK THUMB -->
						<div class="work-thumb">
							<a :href="thumb4link" class="image-popup">
								<img :src="thumb4img" class="img-responsive" alt="Work">
							</a>
						</div>
						<h4>{{thumb4Title}}</h4>
					</div>

				</div>
			</div>
		</section>
</template>

<script>
export default {
  name: "homeneWork",
  props:['anchorTarget3','workTitle','workDesc','thumb1Title','thumb1img','thumb1link','thumb2Title','thumb2img','thumb2link','thumb3Title','thumb3img','thumb3link','thumb4Title','thumb4img','thumb4link']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
