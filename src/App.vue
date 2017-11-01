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
								 :aboutTitle="aboutTitle" 
								 :aboutIntro="aboutIntro"
								 :aboutParas="aboutParas"
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
		<homeneSkill :skillTitle="skillTitle" 
								 :skillDesc="skillDesc" 
								 :bar1Title="bar1Title" 
								 :bar1Width="bar1Width" 
								 :bar2Title="bar2Title" 
								 :bar2Width="bar2Width" 
								 :bar3Title="bar3Title" 
								 :bar3Width="bar3Width">
		</homeneSkill>

		<!-- WORK SECTION -->
		<homeneWork :anchorTarget3="navItems[2]['id']"
								:workTitle="workTitle"
								:workDesc="workDesc" 
								:thumb1Title="thumb1Title" 
								:thumb1img="thumbs[0]['src']" 
								:thumb1link="thumbs[0]['link']"
								:thumb2Title="thumb2Title" 
								:thumb2img="thumbs[1]['src']" 
								:thumb2link="thumbs[1]['link']"
								:thumb3Title="thumb3Title" 
								:thumb3img="thumbs[2]['src']" 
								:thumb3link="thumbs[2]['link']"
								:thumb4Title="thumb4Title" 
								:thumb4img="thumbs[3]['src']" 
								:thumb4link="thumbs[3]['link']">
		</homeneWork>

		<!-- CONTACT SECTION -->
		<homeneContact :anchorTarget4="navItems[3]['id']"
									 :contactTitle="contactTitle"
									 :contactDesc="contactDesc"
									 :field1Name="field1Name"
									 :field1Type="field1Type"
									 :field2Name="field2Name"
									 :field2Type="field2Type"
									 :field3Name="field3Name"
									 :field3Type="field3Type"
									 :textAreaFieldName="textAreaFieldName"
									 :buttonName="buttonName">
		</homeneContact>
		<homeneFooter :footerText="footerText">
		</homeneFooter>
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
import homeneFooter from './components/homeneFooter'
export default {
  name: 'app',
  data(){
	  return siteConfig
  },
  components: {
	homeneHeader,
	homeneHome,
	homeneAbout,
	homeneSkill,
	homeneWork,
	homeneContact,
	homeneFooter
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