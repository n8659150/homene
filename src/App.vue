<!--<template>
  <div id="app">
    <img src="./assets/logo.png">
    <HelloWorld/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>-->

<template>
	<div id="app">
		<!-- PRE LOADER -->
		<div class="preloader" :class="{hideSpinner:pageLoaded}">
			<div class="spinner">
				<span class="spinner-rotate"></span>
			</div>
		</div>


		<!-- NAVIGATION SECTION -->
		<homeneHeader siteTitle="校长不读书" navItem1="Home" anchorMapping1="home" navItem2="About Jack Li" anchorMapping2="about" navItem3="My Works"
			anchorMapping3="work" navItem4="Contact" anchorMapping4="contact">
		</homeneHeader>


		<!-- HOME SECTION -->
		<homeneHome anchorTarget1="home" :profileImg="profileImg" :description="description">
		</homeneHome>
		<!-- ABOUT SECTION -->
		<homeneAbout anchorTarget2="about" :image1="image1" :image2="image2" :image3="image3" :image4="image4" :image5="image5"></homeneAbout>

		<!-- SKILL SECTION -->
		<homeneSkill></homeneSkill>
		<!-- WORK SECTION -->
		<homeneWork anchorTarget3="work"></homeneWork>
		<!-- CONTACT SECTION -->
		<homeneContact anchorTarget4="contact"></homeneContact>
	</div>
</template>

<script>
import homeneHeader from './components/homeneHeader'
import homeneHome from './components/homeneHome'
import homeneAbout from './components/homeneAbout'
import homeneSkill from './components/homeneSkill'
import homeneWork from './components/homeneWork'
import homeneContact from './components/homeneContact'
export default {
  name: 'app',
  data(){
	  return {
			// proloader
			pageLoaded:false,
			//HOME section
		  profileImg:"static/images/profile-image.jpg",
			description:"Hey there, My name is Jack Doe and I'm a Senior Interactive Designer & Web Developer.",
			//ABOUT section
			image1:'static/images/instagram-image1.jpg',
			image2:'static/images/instagram-image2.jpg',
			image3:'static/images/instagram-image3.jpg',
			image4:'static/images/instagram-image4.jpg',
			image5:'static/images/instagram-image5.jpg'
	  }
  },
  components: {
	homeneHeader,
	homeneHome,
	homeneAbout,
	homeneSkill,
	homeneWork,
	homeneContact
  },
	mounted(){
		 setTimeout(() => {
				this.pageLoaded = true;
		}, 1500);
	}
}
</script>

<style scoped>
	.hideSpinner {
		display: none;
	}
</style>