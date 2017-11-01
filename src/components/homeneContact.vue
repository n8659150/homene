<template>
  	<section :id="anchorTarget4">
			<div class="container">
				<div class="row">
					<div class="col-md-12 col-sm-12">
						<div class="wow fadeInUp section-title" data-wow-delay="0.2s">
							<h2>{{contactTitle}}</h2>
							<p>{{contactDesc}}</p>
						</div>
					</div>

					<div class="col-md-12 col-sm-12">
						<!-- CONTACT FORM HERE -->
						<div class="wow fadeInUp" data-wow-delay="0.6s">
							<form id="contact-form">
								<div class="col-md-4 col-sm-4">
									<input :type="field1Type" class="form-control" :name="field1Name" :placeholder="field1Name">
								</div>
								<div class="col-md-4 col-sm-4">
									<input :type="field2Type" class="form-control" :name="field2Name" :placeholder="field2Name">
								</div>
								<div class="col-md-4 col-sm-4">
									<input :type="field3Type" class="form-control" :name="field3Name" :placeholder="field3Name">
								</div>
								<div class="col-md-12 col-sm-12">
									<textarea class="form-control" rows="5" :name="textAreaFieldName" :placeholder="textAreaFieldName"></textarea>
								</div>
								<div class="col-md-offset-9 col-md-3 col-sm-offset-3 col-sm-6">
									<button id="submit" type="submit" class="form-control" name="submit">{{buttonName}}</button>
								</div>
							</form>
						</div>
					</div>
				</div>
			</div>
		</section>
</template>

<script>
export default {
  name: "homeneContact",
  props:['anchorTarget4','contactTitle','contactDesc','field1Name','field1Type','field2Name','field2Type','field3Name','field3Type','textAreaFieldName','buttonName']
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
