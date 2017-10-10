<template>
  <div id="portfolio">
    <!-- <h1>{{ msg }}</h1> -->
    <h2>{{msg}}</h2>
    <v-layout column wrap class="my-5" align-center>
      <!-- <v-flex xs12 sm4 class="my-3">
         <div class="text-xs-center">
           <h2 class="headline">The best way to start developing</h2>
           <span class="subheading">
             Cras facilisis mi vitae nunc 
           </span>
         </div>
       </v-flex> -->
      <v-flex xs12>
        <v-container grid-list-xl>
          <v-layout row wrap align-center>
            <v-flex xs12 md4>
              <v-card class="elevation-0 transparent">
                  <v-card-text class="text-xs-center">
                    <!-- <v-icon x-large class="black--text text--lighten-2">color_lens</v-icon> -->
                    <img src="http://res.cloudinary.com/dmyvekzok/image/upload/c_scale,w_300/v1502836114/Screen_Shot_2017-08-15_at_4.25.54_PM_ygl0us.png"></img>
                  </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline text-xs-center">Inspire</div>
                  </v-card-title>
                  <v-card-text>
                    Example of a project that accesses several API's called through several services and controllers to provide a daily landing page.
                    Data is persistent through a Node server deployed to Heroku. 
                  </v-card-text>
                </v-card>
            </v-flex>
            <v-flex xs12 md4>
              <v-card class="elevation-0 transparent">
                <v-card-text class="text-xs-center">
                  <!-- <v-icon x-large class="black--text text--lighten-2">flash_on</v-icon> -->
                  <img src="http://res.cloudinary.com/dmyvekzok/image/upload/c_scale,w_300/v1507606013/Screen_Shot_2017-10-09_at_9.26.17_PM_ft8vks.png"></img>
                </v-card-text>
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline">Fast development</div>
                </v-card-title>
                <v-card-text>
                  Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. Pellentesque habitant morbi tristique senectus
                  et netus et malesuada fames ac turpis egestas. Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum
                  tincidunt. Suspendisse potenti.
                </v-card-text>
              </v-card>
            </v-flex>
            <v-flex xs12 md4>
              <v-card class="elevation-0 transparent">
                <v-card-text class="text-xs-center">
                  <v-icon x-large class="black--text text--lighten-2">build</v-icon>
                </v-card-text>
                <v-card-title primary-title class="layout justify-center">
                  <div class="headline text-xs-center">Completely Open Sourced</div>
                </v-card-title>
                <v-card-text>
                  Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. Pellentesque habitant morbi tristique senectus
                  et netus et malesuada fames ac turpis egestas. Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum
                  tincidunt. Suspendisse potenti.
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>
      </v-flex>
    </v-layout>
  </div>
</template>

<script>
  export default {
    name: 'portfolio',
    data () {
      return {
        msg: 'Portfolio'
      }

    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  /* h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
} */
</style>