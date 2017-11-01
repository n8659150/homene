<template>
<section id="skill">
			<div class="container">
				<div class="row">

					<div class="col-md-4 col-sm-6">
						<div class="wow fadeInUp section-title" data-wow-delay="0.2s">
							<!-- <h2>Expertise</h2>
							<p>Award winning interdisciplinary Designer & Art director. We have a team who specialise in coding websites.</p>
							 -->
							 <h2>{{skillTitle}}</h2>
							 <p>{{skillDesc}}</p>
						</div>
					</div>

					<div class="col-md-offset-1 col-md-6 col-sm-6">
						<div class="skill-thumb">

							<div class="wow fadeInUp" data-wow-delay="1s">
								<!-- <strong>Graphic Design</strong> -->
								<strong>{{bar1Title}}</strong>
								<!-- <span class="pull-right">95%</span> -->
								<span class="pull-right">{{bar1Width}}</span>
								<div class="progress">
									<div class="progress-bar progress-bar-primary" role="progressbar" aria-valuenow="0" aria-valuemin="0" aria-valuemax="100"
										:style="'width:' + bar1Width"></div>
								</div>
							</div>

							<div class="wow fadeInUp" data-wow-delay="1.2s">
								<strong>{{bar2Title}}</strong>
								<span class="pull-right">{{bar2Width}}</span>
								<div class="progress">
									<div class="progress-bar progress-bar-primary" role="progressbar" aria-valuenow="0" aria-valuemin="0" aria-valuemax="100"
										:style="'width:' + bar2Width"></div>
								</div>
							</div>

							<div class="wow fadeInUp" data-wow-delay="1.4s">
								<strong>{{bar3Title}}</strong>
								<span class="pull-right">{{bar3Width}}</span>
								<div class="progress">
									<div class="progress-bar progress-bar-primary" role="progressbar" aria-valuenow="0" aria-valuemin="0" aria-valuemax="100"
										:style="'width:' + bar3Width"></div>
								</div>
							</div>

						</div>
					</div>

				</div>
			</div>
		</section>
</template>

<script>
export default {
  name: "homeneSkill",
  props:['skillTitle','skillDesc','bar1Title','bar2Title','bar3Title','bar1Width','bar2Width','bar3Width']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
