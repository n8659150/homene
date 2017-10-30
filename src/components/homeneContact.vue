<template>
  	<section id="anchorTarget4">
			<div class="container">
				<div class="row">
					<div class="col-md-12 col-sm-12">
						<div class="wow fadeInUp section-title" data-wow-delay="0.2s">
							<h2>You got projects?</h2>
							<p>Lorem ipsum dolor sit amet, consectetur venenatis tincidunt.</p>
						</div>
					</div>

					<div class="col-md-12 col-sm-12">
						<!-- CONTACT FORM HERE -->
						<div class="wow fadeInUp" data-wow-delay="0.6s">
							<form id="contact-form">
								<div class="col-md-4 col-sm-4">
									<input type="text" class="form-control" name="name" placeholder="Name">
								</div>
								<div class="col-md-4 col-sm-4">
									<input type="email" class="form-control" name="email" placeholder="Email">
								</div>
								<div class="col-md-4 col-sm-4">
									<input type="text" class="form-control" name="name" placeholder="Subject">
								</div>
								<div class="col-md-12 col-sm-12">
									<textarea class="form-control" rows="5" name="message" placeholder="Message"></textarea>
								</div>
								<div class="col-md-offset-9 col-md-3 col-sm-offset-3 col-sm-6">
									<button id="submit" type="submit" class="form-control" name="submit">Send Message</button>
								</div>
							</form>
						</div>
						More Templates <a href="http://www.cssmoban.com/" target="_blank" title="模板之家">模板之家</a> - Collect from <a href="http://www.cssmoban.com/"
							title="网页模板" target="_blank">网页模板</a>
					</div>

				</div>
			</div>
		</section>
</template>

<script>
export default {
  name: "homeneContact",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  },
  props:['anchorTarget4']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
