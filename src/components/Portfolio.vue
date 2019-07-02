<!-- <template>
  <v-card>
    <v-img :src="imgSrc" height="200px">
    </v-img>
    <v-card-title primary-title>
      <div>
        <div class="headline">{{title}}</div>
        <span class="grey--text">{{body}}</span>
      </div>
    </v-card-title>
  </v-card>
</template>

<script>
export default {
	name: 'Portfolio',
	props: {
		date: {type: String},
		title: {type: String},
		body: {type: String},
		imgSrc: {type: String},
	},
	data() {
		return {
			//
		}
	}
}
</script> -->

<template>
  <v-timeline>
    <v-timeline-item
      v-for="n in 3"
      :key="n"
      color="red lighten-2"f
      large
    >
      <template v-slot:opposite>
        <span>{{date}}</span>
      </template>
      <v-card class="elevation-2">
        <ImgBanner>
          <div style="line-height:5em;font-size:5em;" slot="text">
            <v-img src="https://source.unsplash.com/random/800x600"></v-img>
          </div>
        </ImgBanner>
        <v-card-title class="headline">Project name : {{title}}</v-card-title>
        <v-card-text>
          content : {{body}}
        </v-card-text>
      </v-card>
    </v-timeline-item>
  </v-timeline>
</template>

<script>
export default {
	name: 'Portfolio',
	props: {
		date: {type: String},
		title: {type: String},
		body: {type: String},
		imgSrc: {type: String},
	},
	data() {
		return {
			//
		}
	}
}
</script>
