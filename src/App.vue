<!-- <template>
  <v-app light>
    <v-navigation-drawer
      persistent
      :mini-variant="miniVariant"
      :clipped="clipped"
      v-model="drawer"
      enable-resize-watcher
    >
      <v-list>
        <v-list-tile
          value="true"
          v-for="(item, i) in items"
          :key="i"
        >
          <v-list-tile-action>
            <v-icon light v-html="item.icon"></v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title v-text="item.title"></v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar fixed>
      <v-toolbar-side-icon @click.stop="drawer = !drawer" light></v-toolbar-side-icon>
      <v-btn
        icon
        light
        @click.stop="miniVariant = !miniVariant"
      >
        <v-icon v-html="miniVariant ? 'chevron_right' : 'chevron_left'"></v-icon>
      </v-btn>
      <v-btn
        icon
        light
        @click.stop="clipped = !clipped"
      >
        <v-icon>web</v-icon>
      </v-btn>
      <v-btn
        icon
        light
        @click.stop="fixed = !fixed"
      >
        <v-icon>remove</v-icon>
      </v-btn>
      <v-toolbar-title v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        icon
        light
        @click.stop="rightDrawer = !rightDrawer"
      >
        <v-icon>menu</v-icon>
      </v-btn>
    </v-toolbar>
    <main>
      <v-container fluid>
        <v-slide-y-transition mode="out-in">
          <v-layout column align-center>
            <img src="/static/v.png" alt="Vuetify.js" class="mb-5">
            <blockquote>
              &#8220;First, solve the problem. Then, write the code.&#8221;
              <footer>
                <small>
                  <em>&mdash;John Johnson</em>
                </small>
              </footer>
            </blockquote>
          </v-layout>
        </v-slide-y-transition>
      </v-container>
    </main>
    <v-navigation-drawer
      temporary
      :right="right"
      v-model="rightDrawer"
    >
      <v-list>
        <v-list-tile @click="right = !right">
          <v-list-tile-action>
            <v-icon light>compare_arrows</v-icon>
          </v-list-tile-action>
          <v-list-tile-title>Switch drawer (click me)</v-list-tile-title>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-footer :fixed="fixed">
      <span>&copy; 2017</span>
    </v-footer>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'bubble_chart', title: 'Inspire' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Vuetify.js'
      }
    }
  }
</script> -->

<template>
  <div id="app">
    <v-app class="orange darken-3">
      <v-toolbar class="orange darken-3">
        <v-toolbar-title v-text="title"></v-toolbar-title>
        <v-spacer></v-spacer>
        <Navbar></Navbar>
      </v-toolbar>
      <main>
        <section>
          <v-parallax src="http://res.cloudinary.com/dmyvekzok/image/upload/v1500673114/20170506_094130_l7hl3j.jpg">
            <!-- <v-layout
             column
             align-center
             justify-center
             class="white--text"
           >
             <img src="assets/vuetify.png" alt="Vuetify.js">
             <h1 class="white--text mb-2 display-3">Parallax Template</h1>
             <div class="headline mb-3 text-xs-center">Powered by Vuetify</div>
             <v-btn
               class="black lighten-2 mt-5"
               dark
               large
               href="/pre-made-themes"
             >
               Get Started
             </v-btn>
           </v-layout> -->
          </v-parallax>
        </section>

        <section>
          <About></About>
        </section>

        <section>
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
                        <v-icon x-large class="black--text text--lighten-2">color_lens</v-icon>
                      </v-card-text>
                      <v-card-title primary-title class="layout justify-center">
                        <div class="headline text-xs-center">Material Design</div>
                      </v-card-title>
                      <v-card-text>
                        Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. Pellentesque habitant morbi tristique senectus
                        et netus et malesuada fames ac turpis egestas. Nullam in aliquet odio. Aliquam eu est vitae tellus
                        bibendum tincidunt. Suspendisse potenti.
                      </v-card-text>
                    </v-card>
                  </v-flex>
                  <v-flex xs12 md4>
                    <v-card class="elevation-0 transparent">
                      <v-card-text class="text-xs-center">
                        <v-icon x-large class="black--text text--lighten-2">flash_on</v-icon>
                      </v-card-text>
                      <v-card-title primary-title class="layout justify-center">
                        <div class="headline">Fast development</div>
                      </v-card-title>
                      <v-card-text>
                        Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. Pellentesque habitant morbi tristique senectus
                        et netus et malesuada fames ac turpis egestas. Nullam in aliquet odio. Aliquam eu est vitae tellus
                        bibendum tincidunt. Suspendisse potenti.
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
                        et netus et malesuada fames ac turpis egestas. Nullam in aliquet odio. Aliquam eu est vitae tellus
                        bibendum tincidunt. Suspendisse potenti.
                      </v-card-text>
                    </v-card>
                  </v-flex>
                </v-layout>
              </v-container>
            </v-flex>
          </v-layout>
        </section>


        <section>
          <v-parallax src="https://res.cloudinary.com/dmyvekzok/image/upload/v1507567605/20170505_174549_hfip05.jpg">
            <!-- <v-layout
              column
              align-center
              justify-center
              class="white--text"
            >
              <img src="assets/vuetify.png" alt="Vuetify.js">
              <h1 class="white--text mb-2 display-3">Parallax Template</h1>
              <div class="headline mb-3 text-xs-center">Powered by Vuetify</div>
              <v-btn
                class="black lighten-2 mt-5"
                dark
                large
                href="/pre-made-themes"
              >
                Get Started
              </v-btn>
            </v-layout> -->
          </v-parallax>
        </section>











        <section>
          <v-parallax src="assets/section.jpeg" height="380">
            <v-layout column align-center justify-center>
              <div class="headline white--text mb-3">Web development has never been easier</div>
              <em>Kick-start your application today</em>
              <v-btn class="blue lighten-2 mt-5" dark large href="/pre-made-themes">
                Get Started
              </v-btn>
            </v-layout>
          </v-parallax>
        </section>

        <section>
          <v-container grid-list-xl>
            <v-layout row wrap justify-center class="my-5">
              <v-flex xs12 sm4>
                <v-card class="elevation-0 transparent">
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline">Company info</div>
                  </v-card-title>
                  <v-card-text>
                    Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. Pellentesque habitant morbi tristique senectus
                    et netus et malesuada fames ac turpis egestas. Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum
                    tincidunt. Suspendisse potenti.
                  </v-card-text>
                </v-card>
              </v-flex>
              <v-flex xs12 sm4 offset-sm1>
                <v-card class="elevation-0 transparent">
                  <v-card-title primary-title class="layout justify-center">
                    <div class="headline">Contact us</div>
                  </v-card-title>
                  <v-card-text>
                    Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare.
                  </v-card-text>
                  <v-list class="transparent">
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon class="blue--text text--lighten-2">phone</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content>
                        <v-list-tile-title>777-867-5309</v-list-tile-title>
                      </v-list-tile-content>
                    </v-list-tile>
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon class="blue--text text--lighten-2">place</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content>
                        <v-list-tile-title>Chicago, US</v-list-tile-title>
                      </v-list-tile-content>
                    </v-list-tile>
                    <v-list-tile>
                      <v-list-tile-action>
                        <v-icon class="blue--text text--lighten-2">email</v-icon>
                      </v-list-tile-action>
                      <v-list-tile-content>
                        <v-list-tile-title>john@vuetifyjs.com</v-list-tile-title>
                      </v-list-tile-content>
                    </v-list-tile>
                  </v-list>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </section>

        <!-- <v-footer class="blue darken-2">
         <v-layout row wrap align-center>
           <v-flex xs12>
             <div class="white--text ml-3">
               Made with
               <v-icon class="red--text">favorite</v-icon>
               by <a class="white--text" href="https://vuetifyjs.com" target="_blank">Vuetify</a>
               and <a class="white--text" href="mailto:costa.huang@outlook.com">Costa Huang</a>
             </div>
           </v-flex>
         </v-layout>
       </v-footer> -->
      </main>
    </v-app>
  </div>
</template>
<script>
  import Navbar from './components/Navbar'
  import About from './components/About'
  export default {
    name: 'app',
    components: {
      Navbar,
      About
    },
    data() {
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'bubble_chart', title: 'Inspire' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Zach Springer  >>  Full Stack Developer'
      }
    }
  }
</script>

<style>
</style>