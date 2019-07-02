<template>
  <div>
    <ImgBanner imgSrc="https://source.unsplash.com/5brvJbR1Pn8/1600x900">
      <div style="line-height:1.2em;font-size:1.2em;" slot="text">I</div>
    </ImgBanner>
    <span class="verb"> <span class="question">question</span></span>
    <v-container>

      <!-- Portfolio -->
      <v-layout>
        <Portfolio :limits="3" :load-more="true"></Portfolio>
        <!-- <v-flex xs12>
          <PortfolioList :limits="6" :load-more="true"></PortfolioList>
        </v-flex> -->
      </v-layout>

    </v-container>
  </div>
</template>

<script>
import ImgBanner from '../components/ImgBanner'
import Portfolio from '../components/Portfolio'
// import PortfolioList from '../components/PortfolioList'

export default {
	name: 'PortfolioPage',
	components: {
		ImgBanner,
    Portfolio,
		// PortfolioList,
	},
}
</script>
