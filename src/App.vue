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
		<homeneHeader :siteTitle="siteTitle" 
									:navItem1="navItems[0]['name']" 
									:anchorMapping1="navItems[0]['id']" 
									:navItem2="navItems[1]['name']" 
									:anchorMapping2="navItems[1]['id']" 
									:navItem3="navItems[2]['name']"
									:anchorMapping3="navItems[2]['id']" 
									:navItem4="navItems[3]['name']" 
									:anchorMapping4="navItems[3]['id']">
		</homeneHeader>


		<!-- HOME SECTION -->
		<homeneHome :anchorTarget1="navItems[0]['id']" :profileImg="profileImg" :description="description">
		</homeneHome>
		<!-- ABOUT SECTION -->
		<homeneAbout :anchorTarget2="navItems[1]['id']"
								 aboutTitle="A Little Bit Of My Story" 
								 aboutIntro="Senior Interactive Designer & Web Developer at yourdreamjob.com"
								 aboutParas="Award winning interdisciplinary Designer & Art director. We have a team who specialise in coding websites and themes
									perfect blend of style and function for a wide range of interactive product design."
								 :image1="images[0]['src']" 
								 :image2="images[1]['src']" 
								 :image3="images[2]['src']" 
								 :image4="images[3]['src']" 
								 :image5="images[4]['src']"
								 :image1Link="images[0]['link']"
								 :image2Link="images[1]['link']"
								 :image3Link="images[2]['link']"
								 :image4Link="images[3]['link']"
								 :image5Link="images[4]['link']"
								 >
		</homeneAbout>

		<!-- SKILL SECTION -->
		<homeneSkill skillTitle="Expertise" 
								 skillDesc="Award winning interdisciplinary Designer & Art director. We have a team who specialise in coding websites." 
								 bar1Title="Graphic Design" 
								 bar1Width="90%" 
								 bar2Title="Minimal Themes" 
								 bar2Width="100%" 
								 bar3Title="Media & Photography" 
								 bar3Width="75%">
		</homeneSkill>
		<!-- WORK SECTION -->
		<homeneWork :anchorTarget3="navItems[2]['id']"></homeneWork>
		<!-- CONTACT SECTION -->
		<homeneContact :anchorTarget4="navItems[3]['id']"></homeneContact>
	</div>
</template>

<script>
// 内容配置
import siteConfig from '../static/siteConfig'
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
			siteTitle:'Homene',
			navItems:[
					{id:'home',name:'Home'},
					{id:'about',name:'About Me'},
					{id:'work',name:'My Work'},
					{id:'contact',name:'Contact'}
			],
		  profileImg:'static/images/profile-image.jpg',
			description:"Hey there, My name is Jack Doe and I'm a Senior Interactive Designer & Web Developer.",
			//ABOUT section
			images:[
				{src:'static/images/instagram-image1.jpg',link:'https://www.instagram.com/p/cqED9yjN0j/'},
				{src:'static/images/instagram-image2.jpg',link:'https://www.instagram.com/p/enL0SsDN51/'},
				{src:'static/images/instagram-image3.jpg',link:'https://www.instagram.com/p/apOuRTDNwJ/'},
				{src:'static/images/instagram-image4.jpg',link:'https://www.instagram.com/p/ZXIj33jN2v/'},
				{src:'static/images/instagram-image5.jpg',link:'https://www.instagram.com/p/Xwev1FjN9-/'}
			]
			
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